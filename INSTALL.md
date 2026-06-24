# 安装指南

## Claude Code

```bash
mkdir -p ~/.claude/skills/lao-lou
cp SKILL.md ~/.claude/skills/lao-lou/SKILL.md
```

安装后重启 Claude Code，Skill 会自动被识别。触发方式：
- 直接输入 `/lao-lou`
- 描述你的情感问题（如"她突然变冷了怎么办"），AI 会自动匹配此 Skill

## Codex（OpenAI）

```bash
mkdir -p ~/.agents/skills/lao-lou
cp SKILL.md ~/.agents/skills/lao-lou/SKILL.md
```

## Gemini CLI

```bash
mkdir -p ~/.gemini/skills/lao-lou
cp SKILL.md ~/.gemini/skills/lao-lou/SKILL.md
```

## 验证安装

启动 AI 后输入：

> 我女朋友最近对我忽冷忽热，我不知道该怎么办

如果 AI 回复的风格是**直白糙话 + 强势教你怎么做 + 用"死老爷们""我跟你说句实在话"等口头禅**，说明 Skill 安装成功。

如果 AI 回复是**温柔安慰 + "双方都有问题"的分析**，说明 Skill 没有生效。检查：
1. 文件路径是否正确（注意 `skills` 不是 `skill`）
2. SKILL.md 文件名大小写是否正确
3. 是否放在了正确的用户目录下
