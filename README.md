# 穿搭与摄影提示词技能

两个独立安装的 Codex 技能：

| 技能目录 | 用途 | 来源 |
| --- | --- | --- |
| `skills/outfit-stylist` | 单品搭配、整套造型建议与搭配诊断；原版默认可生成中文 OOTD 搭配板，也接受仅文字要求 | [kingqiu/outfit-stylist-skill](https://github.com/kingqiu/outfit-stylist-skill) |
| `skills/outfit-photo-prompter` | 围绕服装设计人物、搭配和生活场景，编写穿搭摄影提示词；默认不生图 | mumu0214-chou 的自编技能，本次上传保留本地现有版本 |

## 下载与安装

在 Codex 中复制下面的提示词：

```text
使用 $skill-installer，从 https://github.com/mumu0214-chou/outfit-skills 安装这两个技能目录：
1. skills/outfit-stylist
2. skills/outfit-photo-prompter
请完整安装各自的 references、assets、agents，以及随附的 LICENSE 和 SOURCE.md（如有）。安装后确认两个 SKILL.md 都存在，并告诉我调用名称。
```

也可以[下载整个仓库 ZIP](https://github.com/mumu0214-chou/outfit-skills/archive/refs/heads/main.zip)。手动安装时，把 `skills` 下的两个技能目录分别放入支持本地技能的 Agent 技能目录，保留每个目录的完整内容。

## 使用示例

先做文字搭配：

```text
使用 $outfit-stylist，根据我提供的一件衣服设计整套搭配。直接由 AI 设计，不搜索穿搭素材。先只输出一套主方案、选择理由和一个轻量替换，不生成图片。
```

再把确定的搭配转成摄影提示词：

```text
使用 $outfit-photo-prompter，沿用刚才已经确定的搭配，为其编写自然街拍提示词。只写提示词，不生成图片。商品图用于保留服装款式；如果另有摄影参考图，按我说明的范围借鉴。
```

两个技能的生成默认不同，上述使用示例明确选择了文字模式。生成图片需要所在环境支持图像生成；仅做搭配和提示词不需要生成图片。

## 来源与授权

`outfit-stylist` 原作者为 kingqiu，来自上面链接的公开项目。本目录保留原技能、参考文档与模板，并补充了完整的 [PolyForm Noncommercial License 1.0.0](skills/outfit-stylist/LICENSE) 和[来源说明](skills/outfit-stylist/SOURCE.md)。其非商业使用条件继续适用；公开镜像不会改变原项目授权。

各目录的来源与许可分别适用。本仓库没有用统一许可证替代第三方许可证。
