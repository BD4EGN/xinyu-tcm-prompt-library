# 🏥 信羽中医养生 Prompt 模板库

> 专为中医养生 / 大健康类小红书内容优化的 GPT Image 2 Prompt 模板库
> 基于社区最佳实践提炼，每日生产 300+ 张小红书图片

---

## 📖 说明

本库收集并整理了针对 **中医养生 / 大健康 / 私域运营** 场景的 GPT Image 2 高精度图片生成提示词模板。

### 参考来源

本库参考了以下三个 Fork 的社区 Prompt 库：

| 仓库 | 地址 |
|------|------|
| awesome-gptimage2-prompts (3000+ prompts) | [BD4EGN/awesome-gptimage2-prompts](https://github.com/BD4EGN/awesome-gptimage2-prompts) |
| awesome-gpt-image-2 (2000+ prompts) | [BD4EGN/awesome-gpt-image-2](https://github.com/BD4EGN/awesome-gpt-image-2) |
| awesome-gpt-image-2-API-and-Prompts (700+ 案例) | [BD4EGN/awesome-gpt-image-2-API-and-Prompts](https://github.com/BD4EGN/awesome-gpt-image-2-API-and-Prompts) |

---

## 🗂️ 目录结构

```
xinyu-tcm-prompt-library/
├── README.md                          ← 本文件
├── prompt-engineering-guide.md        ← GPT Image 2 Prompt 工程指南
│
├── templates/                         ← 核心模板
│   ├── cover-kaoyan.md               ← 知识科普卡（通用模板）
│   ├── cover-single-product.md       ← 单品深扒卡
│   ├── cover-comparison.md           ← 对比测评卡
│   ├── cover-tips.md                 ← 养生小贴士卡
│   ├── cover-recipe.md               ← 食疗方卡
│   ├── cover-acupoint.md             ← 穴位科普卡
│   └── cover-qa.md                   ← 问答互动卡
│
├── categories/                        ← 按选题分类的 Prompt
│   ├── dampness.md                   ← 祛湿主题
│   ├── spleen-stomach.md             ← 脾胃调理
│   ├── sleep.md                      ← 失眠/睡眠
│   ├── women-health.md               ← 女性健康
│   ├── skin-care.md                  ← 美容养颜
│   ├── liver-detox.md                ← 养肝护肝
│   ├── kidney-tonify.md              ← 补肾益精
│   └── children-health.md            ← 儿童健康
│
├── styles/                            ← 视觉风格参考
│   ├── new-chinese-style.md          ← 新中式风格
│   ├── minimalist.md                 ← 极简杂志风
│   ├── warm-healing.md               ← 温暖疗愈风
│   ├── hand-drawn.md                 ← 手绘插画风
│   └── traditional-ink.md            ← 水墨国风
│
├── color-palettes/                    ← 配色方案
│   ├── tea-warm.md                   ← 暖茶色系
│   ├── herb-green.md                 ← 草本绿系
│   ├── golden-amber.md               ← 琥珀金系
│   └── medicine-wood.md              ← 药木棕系
│
├── product-prompts/                   ← 信羽产品专属 Prompt
│   ├── qu-shi-gao.md                 ← 祛湿膏专用
│   ├── jian-pi-yang-wei-gao.md       ← 健脾养胃膏专用
│   ├── zi-yin-shi-hu-gao.md          ← 滋阴石斛膏专用
│   ├── shu-san-san-jie-gao.md        ← 疏肝散结膏专用
│   ├── qu-shi-cha.md                 ← 祛湿茶专用
│   ├── yang-gan-hu-gan-cha.md        ← 养肝护肝茶专用
│   └── san-jiao-cha.md               ← 三焦茶专用
│
└── batch-workflow/                    ← 批量生产工作流
    ├── daily-3-pieces.md             ← 日更 3 条 SOP
    ├── calendar-template.md          ← 内容日历模板
    └── tcm-rag-pipeline.md           ← RAG → Prompt → 图片 全自动流水线
```

---

## 🎯 核心模板速览

### 1. 知识科普卡（通用）
适合：每日知识科普类笔记
```
[主体] 一个精美的陶瓷茶杯放在竹制茶盘上，
       旁边放着中药材（枸杞/菊花/陈皮等），杯子冒着热气
[场景] 阳光透过竹帘洒在木桌上，背景是虚化的中式书房，
       有书法卷轴和盆栽绿植
[风格] 新中式极简，小红书封面，暖米色+淡茶色+自然绿
[构图] 竖屏3:4，主体居中偏下，上方留白40%放标题
[用光] 柔和的晨光从左侧斜射，温暖金色调
[文字] 标题："XXXX" 白色粗体，字占宽度60%
       副标："XXXXXXXX" 浅灰小字
       无其他文字
```

### 2. 单品深扒卡
适合：产品推荐类笔记
```
[主体] 产品实拍（罐装膏/茶包/粉剂），放在天然亚麻布上，
       旁边搭配对应的中药材原料展示
[场景] 自然光台面，木纹背景或大理石纹理，
       干净简洁但不失温度
[风格] 高端产品摄影风，微距细节，质感突出
[构图] 竖屏3:4，产品位于黄金分割点，
       周围留有呼吸空间
[用光] 柔和的侧逆光，突出产品质感和药材纹理
[文字] 标题："XXXXX" 产品名或核心卖点
       副标：适用人群或功效关键词
```

### 3. 对比测评卡
适合：A vs B 对比、适合/不适合、真/假辨别
```
[主体] 左右分屏布局：
       左半——绿色背景区域（适合/正确/建议）
       右半——灰色背景区域（不适合/错误/不建议）
[场景] 干净的纯色基底，中间用渐变或细线分隔
[风格] 极简信息图风格，清晰可读
[构图] 竖屏3:4，左右1:1分割
[文字] 左侧标题绿色："✅ 适合/正确做法"
       右侧标题灰色："❌ 不适合/错误做法"
       下方各配2-3个要点文字
```

---

## 🚀 快速开始

1. 浏览 `templates/` 找到适合的内容类型模板
2. 打开相应模板，替换主体/文字
3. 如需选题参考，在 `categories/` 找到对应主题
4. 如需风格调整，在 `styles/` 参考不同的视觉风格
5. 如需配色方案，在 `color-palettes/` 选色板

### 批量生产 SOP

详见 `batch-workflow/daily-3-pieces.md`，实现每天 3 条的自动化生产流程。

---

## 🧠 Prompt 核心方法论

GPT Image 2 不是关键词匹配引擎，而是带推理能力的原生多模态模型。

关键技巧：
1. **分层法**：主体 → 场景 → 风格 → 构图 → 用光 → 文字，逐层叠加
2. **文字加引号**：精确文字必须用引号括起来
3. **反文字防护**：末尾加"图片中无其他文字标签水印"
4. **6 元素结构**：主体 > 场景 > 风格 > 构图 > 用光 > 文字（按优先级排序）
5. **不超过 3 次迭代**：不满意就重写 Prompt，别在同一对话里反复修

详细方法论见 `prompt-engineering-guide.md`

---

## 🔗 相关链接

- [awesome-gptimage2-prompts](https://github.com/BD4EGN/awesome-gptimage2-prompts) (3000+ prompts)
- [awesome-gpt-image-2](https://github.com/BD4EGN/awesome-gpt-image-2) (2000+ prompts, 16 languages)
- [awesome-gpt-image-2-API-and-Prompts](https://github.com/BD4EGN/awesome-gpt-image-2-API-and-Prompts) (700+ cases)
- [GPT Image 2 Prompt Guide (Pixo)](https://pixo.video/blog/gpt-image-2-prompt-guide)
- [GPT Image 2 Official Prompts](https://gptimage2.github.io/gpt-image-2-prompts.html)
