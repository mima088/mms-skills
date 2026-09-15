---
name: mms-kuapingtai-qiaojie
description: 【Cross-platform Bridge】米妈技能跨平台桥接。把 MMS 的 skill 转成可在 Codex、WorkBuddy、TraeWork CN、豆包上安装使用的格式。当用户说“装到别的平台”“跨平台”“导出给豆包”时使用。
---

# 米妈技能跨平台桥接

## 各平台对应格式
- Codex：`SKILL.md`（YAML frontmatter + body），放 `~/.codex/skills/技能名/`；
- WorkBuddy：支持从 GitHub 仓库地址安装 skill；
- TraeWork CN：支持从 GitHub 仓库地址安装 skill；
- 豆包：粘贴到智能体“人设/系统提示词”。

## 转换步骤
1. 去掉 Codex 的 YAML frontmatter，保留 body；
2. 把路径引用改成平台能读到的路径或直接内嵌；
3. 去掉平台不支持的命令/脚本，只留纯文本指令；
4. 给每个平台出一份可粘贴的纯文本版本。

## 输出
- 一个通用 Markdown（可粘贴）；
- 各平台注意点（哪些要删、哪些要改）。

## 完成后
按 `mms` 总入口的「技能联动路由表」，主动给出 1 个最相关的下一步建议（最多 1 个，不刷屏）。

