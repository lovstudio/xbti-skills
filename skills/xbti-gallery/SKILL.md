---
name: lov-xbti-gallery
category: xBTI
tagline: "Browse all community-created BTI personality tests at xbti.example.com."
description: >
  Browse the XBTI Gallery — all community-created BTI personality tests at xbti.example.com.
  Trigger when user says "XBTI Gallery", "xbti-gallery", "BTI列表", "浏览人格测试",
  "show BTI cases", or wants to see available BTI variants.
allowed-tools: [Bash, Read]
license: MIT
compatibility: Requires `gh` CLI for listing cases.
metadata:
  author: contributors
  version: "1.0.2"
  tags: bti personality-test gallery xbti
---

# xbti-gallery — Browse Community BTI Tests

Open the XBTI Gallery and list all community-created BTI personality tests.

## When to Use

- User wants to browse existing BTI personality tests
- User says "打开 XBTI Gallery" or "show me BTI cases"
- User wants to see what others have created before making their own

## Workflow

### Step 1: Open Gallery

If the user did not specify whether to open the web gallery or list repository
cases, use `AskUserQuestion` to choose the mode. If they explicitly asked to
open or list, proceed directly.

```bash
open https://example.com/community
```

### Step 2: List Available Cases

Fetch and display all BTI variants from the repository:

```bash
gh api repos/skill-publisher/XBTI/contents/cases 2>/dev/null | python3 -c "
import json, sys
try:
    items = json.load(sys.stdin)
    if isinstance(items, list):
        for item in items:
            if item.get('type') == 'dir':
                print(f'  - {item[\"name\"]}')
    else:
        print('  (no cases yet)')
except:
    print('  (unable to fetch)')
"
```

If no cases exist, tell the user: "Gallery 还没有案例，用 `/lov-xbti-creator` 创建一个并提交吧！"

## Runtime context (shared)

运行前读取本 Skill 包的 `skill.yaml`，由宿主提供 `skill-runtime/v1` 上下文。字段解析顺序为：当前请求、项目上下文、个人 Preferences、品牌 Profile、通用默认值。

- 只使用 Manifest 声明的字段；Profile 保存公开品牌事实，Preferences 保存个人工作偏好。
- `required: true` 字段缺失时，按 Manifest 的问题配置向用户提出一个聚焦问题；用户明确同意后再保存回答。
- 报错提供可复制的 `context_id`、字段路径与来源，诊断内容避开秘密、完整私人路径和原始配置。
