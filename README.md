<h1 align="center">Lovstudio xBTI Skills</h1>

<p align="center">
  <strong>Lovstudio xBTI 人格测试相关的 Claude Code 技能子索引。</strong><br>
  <sub>由 <a href="https://lovstudio.ai">Lovstudio</a> 出品 · <a href="https://xbti.lovstudio.ai">xbti.lovstudio.ai</a></sub>
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

本仓库是 Lovstudio 技能体系中**围绕 xBTI（BTI 人格测试定制与画廊）**的子索引，是 [`lovstudio/skills`](https://github.com/lovstudio/skills) 主索引的专题分支。

配合 [xbti.lovstudio.ai](https://xbti.lovstudio.ai) 使用：从定制自己的 BTI（如 LBTI、FBTI）到在社区画廊里浏览发布作品。

每个技能仍然在自己的独立仓库 `github.com/lovstudio/{name}-skill` 里。本仓库只维护索引与镜像。

## 技能列表

<!-- COUNT:START -->
> **2 个技能** — 2 个免费 + 0 个付费。
<!-- COUNT:END -->

<!-- SKILLS:START -->
| | 技能 | 描述 |
|---|---|---|
| **人格测试** | | |
| ![Free](https://img.shields.io/badge/Free-green) | [xBTI 测试定制 · `xbti-creator`](https://github.com/lovstudio/xbti-creator-skill) | 定制属于你自己的 BTI 人格测试（LBTI、FBTI 等），题目、结果、头像全自动生成。 |
| ![Free](https://img.shields.io/badge/Free-green) | [xBTI 画廊 · `xbti-gallery`](https://github.com/lovstudio/xbti-gallery-skill) | 浏览社区在 xbti.lovstudio.ai 上发布的所有 BTI 人格测试。 |
<!-- SKILLS:END -->

<sub>上表由 [`scripts/render-readme.py`](scripts/render-readme.py) 从 [`skills.yaml`](skills.yaml) 自动生成。请编辑 `skills.yaml`，不要手动改表格。</sub>

## 安装

**通过 `npx skills`**（vercel-labs CLI）：

```bash
npx skills add lovstudio/xbti-skills
```

**通过 Claude Code 原生 marketplace**：

```
/plugin marketplace add lovstudio/xbti-skills
/plugin install xbti@lovstudio-xbti
```

## 相关索引

- [`lovstudio/skills`](https://github.com/lovstudio/skills) — Lovstudio 所有技能的主索引
- [`lovstudio/dev-skills`](https://github.com/lovstudio/dev-skills) — 开发者 & 元技能

## 许可证

- **本索引仓库**：MIT
- **免费技能**：MIT（详见各仓库的 LICENSE）

---

<p align="center">
  <sub>使用 <a href="https://claude.com/claude-code">Claude Code</a> 构建 · 由 <a href="https://lovstudio.ai">Lovstudio</a> 出品</sub>
</p>
