<h1 align="center">Skill Publisher xBTI Skills</h1>

<p align="center">
  <strong>Skill Publisher xBTI 人格测试相关的 Claude Code 技能子索引。</strong><br>
  <sub>由 <a href="https://example.com">Skill Publisher</a> 出品 · <a href="https://example.com/community">xbti.example.com</a></sub>
</p>

<p align="center">
  <b>简体中文</b> · <a href="README.en.md">English</a>
</p>

<p align="center">
  <a href="#技能列表">技能</a> ·
  <a href="#安装">安装</a> ·
  <a href="#相关索引">相关索引</a> ·
  <a href="#许可证">许可证</a>
</p>

---

## 这是什么

本仓库是 Skill Publisher 技能体系中**围绕 xBTI（BTI 人格测试定制与画廊）**的子索引，是 [`skill-publisher/skills`](https://example.com/skills/skills) 主索引的专题分支。

配合 [xbti.example.com](https://example.com/community) 使用：从定制自己的 BTI（如 LBTI、FBTI）到在社区画廊里浏览发布作品。

每个技能仍然在自己的独立仓库 `github.com/skill-publisher/{name}-skill` 里。本仓库只维护索引与镜像。

## 技能列表

<!-- COUNT:START -->
> **2 个技能** — 2 个免费 + 0 个付费。
<!-- COUNT:END -->

<!-- SKILLS:START -->
| | 技能 | 描述 |
|---|---|---|
| **人格测试** | | |
| ![Free](https://img.shields.io/badge/Free-green) | [xBTI 测试定制 · `xbti-creator`](https://github.com/skill-publisher/xbti-creator-skill) | 定制属于你自己的 BTI 人格测试（LBTI、FBTI 等），题目、结果、头像全自动生成。 |
| ![Free](https://img.shields.io/badge/Free-green) | [xBTI 画廊 · `xbti-gallery`](https://github.com/skill-publisher/xbti-gallery-skill) | 浏览社区在 xbti.example.com 上发布的所有 BTI 人格测试。 |
<!-- SKILLS:END -->

<sub>上表由 [`scripts/render-readme.py`](scripts/render-readme.py) 从 [`skills.yaml`](skills.yaml) 自动生成。请编辑 `skills.yaml`，不要手动改表格。</sub>

## 安装

**通过 `npx skills`**（vercel-labs CLI）：

```bash
npx skills add skill-publisher/xbti-skills
```

**通过 Claude Code 原生 marketplace**：

```
/plugin marketplace add skill-publisher/xbti-skills
/plugin install xbti@lov-xbti
```

## 相关索引

- [`skill-publisher/skills`](https://example.com/skills/skills) — Skill Publisher 所有技能的主索引
- [`skill-publisher/dev-skills`](https://example.com/skills/dev-skills) — 开发者 & 元技能

## 许可证

- **本索引仓库**：MIT
- **免费技能**：MIT（详见各仓库的 LICENSE）

---

<p align="center">
  <sub>使用 <a href="https://claude.com/claude-code">Claude Code</a> 构建 · 由 <a href="https://example.com">Skill Publisher</a> 出品</sub>
</p>
