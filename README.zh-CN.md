# vinyl-wallpaper-generator

[English](README.md) | [简体中文](README.zh-CN.md)

把一张照片、一段记忆、一句话、一种情绪、一个故事、一个物件或地点，转化成**两张配套的虚构黑胶主题手机壁纸**——一张封面艺术版，一张带唱臂的唱片版。

基于 Agent Skill（SKILL.md 规范）构建。

## 示例

| 封面壁纸 | 唱片壁纸 |
|:---:|:---:|
| ![封面壁纸示例](examples/cover-wallpaper.png) | ![唱片壁纸示例](examples/record-wallpaper.png) |

两张均为 **9:19.6 竖版**，浅色渐变背景、极细曲线装饰、无任何系统 UI、底部极简播放器进度条。唱片版包含唱臂，唱针落在唱片外圈纹路。

## 功能

给定一张源照片或一段文字想法，技能会自动完成：分析源材料提取视觉元素 → 构建虚构黑胶发行（艺人名、专辑名、厂牌、曲目列表，艺人名会联网验证避免与真实音乐人冲突）→ 设计视觉系统 → 并行生成两张壁纸。

## 安装

直接告诉 AI 助手帮你安装即可，无需手动克隆：

> *"帮我安装 vinyl-wallpaper-generator 这个技能，仓库地址是 https://github.com/Irisnotiris/vinyl-wallpaper-generator"*

助手会自动把仓库克隆到你的技能目录。

## 使用

自然语言调用即可：

- *"用 vinyl-wallpaper-generator 把这张照片做成壁纸"*
- *"把这段记忆做成两张黑胶壁纸"*
- *"把'我们活着如同独自做梦'做成两张黑胶手机壁纸"*

## 仓库结构

```
vinyl-wallpaper-generator/
├── SKILL.md                          # 技能主文档（工作流 + 设计规范）
├── README.md                         # 英文说明
├── README.zh-CN.md                   # 中文说明
├── LICENSE
├── references/
│   └── prompt_templates.md           # 图片生成 prompt 模板
└── examples/
    ├── cover-wallpaper.png
    └── record-wallpaper.png
```

## 致谢

本技能灵感来源于 [liigoQi](https://github.com/liigoQi) 的 [vinyl-image-generator](https://github.com/liigoQi/vinyl-image-generator)，并在此基础上扩展为手机壁纸版本。

## 许可证

MIT
