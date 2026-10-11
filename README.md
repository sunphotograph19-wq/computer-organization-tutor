# Computer Organization Tutor

一个面向《计算机组成原理》课程的 Agent Skill，适合将教师 PPT / PDF、指定教材、习题与答案整理成适合自学、补课、考试复习和 Obsidian 长期积累的中文笔记。

## 特点

- 以教师 PPT 确定课程范围
- 用习题反推考试重点
- 用指定教材补充陌生概念和推理断层
- 对知识点进行 S / A / B / C 考点分级
- 对陌生概念按“定义 → 通俗理解 → 为什么需要 → 工作过程 → 例子 → 易错点 → 怎么考”展开
- 针对《计算机组成原理》强化 ALU、寄存器、总线、补码、溢出、移位、浮点数、Cache、CPU 数据通路等内容
- 默认生成 Obsidian 兼容 Markdown
- 支持 Properties、Wikilinks、Callout、附件嵌入、掌握度 Checkbox、MOC 与考前速记

## 仓库结构

```text
computer-organization-tutor/
├── SKILL.md
├── README.md
└── templates/
    ├── Obsidian-章节笔记模板.md
    └── 计算机组成原理-MOC模板.md
```

## 推荐使用方式

将某一章节的课程资料放在同一项目中，例如：

```text
第02章/
├── PPT/
├── 习题/
├── 教材/
└── notes/
```

然后向 Agent 提出类似请求：

```text
我没有完整听这一节课。
请结合本节 PPT、指定教材和习题帮我补课。
先建立知识框架，再详细解释陌生概念；
根据习题判断考试重点并进行 S/A/B/C 分级；
最后输出适合 Obsidian 的章节笔记、复习小结和考前30秒速记。
```

## Obsidian 输出

Skill 默认优先使用 Obsidian 原生 Markdown 能力，包括：

- YAML Properties
- `[[Wikilinks]]`
- `![[attachments]]`
- Callout
- Checkbox
- Markdown 表格
- MOC（Map of Content）

默认不依赖 Dataview、Templater、Tasks 等第三方插件。

## 安装到 Amp

如果你的 Amp 支持从 GitHub 安装 Agent Skills，可将本仓库作为 Skill 来源安装。安装后，在包含课程资料的项目中调用 `computer-organization-tutor` 即可。

## 适用场景

当前版本主要针对《计算机组成原理》，尤其适合：

- 没完整听课，需要根据 PPT 快速补课
- PPT 内容过于简略，需要教材辅助理解
- 希望结合习题判断老师真正重视的考点
- 希望长期使用 Obsidian 整理课程知识库
- 需要章节小结、重点分级、自测与考前速记

## 说明

如果 PPT、教材与习题答案存在差异，Skill 会明确标记资料差异，而不是静默替换课程材料中的表述。
