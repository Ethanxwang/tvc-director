# TVC Director · TVC 广告创意导演

[English](README_en.md)

从产品 brief 到电影级 TVC 关键帧——你的 AI 广告创意导演。

一个将 AI Agent 转化为 **TVC 广告创意导演** 的 Skill，覆盖电视广告和品牌广告的完整创意流程：从产品 brief 到可直接使用的 **Nano Banana Pro** 关键帧提示词和 **Seedance** Multi-Phase 视频脚本。

## 核心特性

- **完整创意流水线** — 从一句话需求到可交付的分镜提示词和视频脚本，全程 AI 驱动
- **8 种 TVC 叙事模型** — 痛点-解决、产品电影化拆解、品牌世界穿梭等，覆盖主流广告叙事
- **电影级视觉系统** — 5 种画风预设（A-E）、12 种场景类型、精确到秒的运镜编排
- **产品+品牌世界双线叙事** — 不只是产品特写，而是产品在真实场景中的交叉剪辑
- **即拷即用** — 产出的提示词可直接粘贴到 Nano Banana Pro / Seedance，无需二次加工

## 成品展示

### 汽车 TVC — 产品电影化拆解

https://github.com/user-attachments/assets/541055ed-d716-4087-86e2-a27d375282ed

### 香水 TVC — 品牌世界穿梭

https://github.com/user-attachments/assets/df2d51af-acc2-4f34-a228-8b35ea754345

## 快速上手：一条汽车 TVC 的诞生

以下是一个真实的端到端案例——从一张参考图到 15 秒成片。

### Step 1 — 给一张参考图 + 一句话需求

> "帮我做一条银色轿跑的 15 秒 TVC"

<img src="https://github.com/user-attachments/assets/0d774888-0dbb-4fb7-a861-ca3116b812b7" width="400" alt="参考图：银色轿跑" />

AI 会自动进入完整创意流：需求拆解 → 创意构思 → 画风确认 → 资产生成 → 分镜 + 视频脚本。

### Step 2 — AI 生成产品多视图提示词 → Nano Banana Pro 出图

AI 输出产品多视图提示词，复制到 Nano Banana Pro（edit 模式，传入参考图），得到标准化的多角度产品图：

<img src="https://github.com/user-attachments/assets/9d97df38-79f1-4a6a-a6bb-0fdbd731faca" width="600" alt="产品多视图" />

### Step 3 — AI 生成 9 宫格分镜提示词 → Nano Banana Pro 出图

AI 输出 3×3 多宫格分镜提示词（包含逐格构图、光影、运镜描述），复制到 Nano Banana Pro（edit 模式，传入多视图 + 环境图），得到完整分镜：

<img src="https://github.com/user-attachments/assets/1ca54c8a-e1c2-4a13-8e67-461ea327f2ab" width="600" alt="9 宫格分镜" />

### Step 4 — AI 生成 Multi-Phase 视频脚本 → Seedance 生成视频

AI 同步输出 Seedance Multi-Phase 视频提示词（5 Phase / 15s），配合多宫格作为首帧 + 产品多视图作为锚定，双图输入 Seedance 生成最终视频。

### 产出物一览

| 产出物 | 工具 | 用途 |
|--------|------|------|
| 产品多视图 | Nano Banana Pro (edit) | 产品锚定，供后续步骤引用 |
| 9 宫格分镜图 | Nano Banana Pro (edit) | 视频首帧 + 视觉校对 |
| Multi-Phase 视频脚本 | Seedance | 生成 15s 成片 |
| 创意方案文档 | — | 完整创意 brief 存档 |

## 设计理念

传统 AI 生成广告往往只是"产品 + 黑底 + 旋转"的无限循环。TVC Director 不同：

- **叙事驱动，而非模板填充** — 先确定叙事模型和创意方向，再生成视觉
- **双世界交叉剪辑** — 产品特写与品牌世界场景交织，像真正的 TVC 一样讲故事
- **精确到秒的运镜设计** — 每一格分镜都有明确的景别、角度、光影和转场逻辑
- **渐进式人机协作** — 每个阶段都可以介入调整，不是一键出片的黑盒

## 三大核心能力

### 1. 产品电影化拆解（Cinematic Product Breakdown）

产品是唯一主角，纯影棚，多 Phase 的产品微电影：

- 零件悬浮拆解/精密组装动画
- 材质微距：金属磨砂纹理、玻璃折射、碳纤维编织
- 精确到秒的运镜编排：极慢拆解 → 爆发旋转 → 悬浮凝视 → 俯冲穿越
- 光影叙事：低调影棚光、侧光勾勒轮廓、光随旋转流动

### 2. 品牌世界穿梭（Brand World Crosscut）

品牌世界和产品世界轮流出场，用 Match Cut 衔接：

- 运动相机 → 跳伞、潜水、滑雪、攀岩
- 越野车 → 盘山弯道、沙漠、雪地
- 每个 Phase 完整待在一个世界里，通过匹配剪辑无缝切换

### 3. 场景内叙事（In-Scene Narrative）

产品始终待在品牌世界中，不跳出去做影棚特写：

- 跑鞋穿在脚上、手表戴在手腕、眼镜架在鼻梁
- 通过运镜手法（低角度追拍、慢动作、景深变化）自然突出产品
- 片尾集中做 Hero Shot 收束

## 安装

### Cursor

```bash
git clone https://github.com/Ethanxwang/tvc-director.git ~/.cursor/skills/tvc-director
```

### Claude Code

```bash
git clone https://github.com/Ethanxwang/tvc-director.git ~/.claude/skills/tvc-director
```

## 工作流程

```
"帮我做一条户外相机的30秒TVC"
        ↓
  Phase 0: 入口模式判断
  Phase 1: 需求拆解（产品/时长）
  Phase 2: TVC 创意构思（2-3 个方向 → 选择 → 完整创意方案）
  Phase 3: 画风确认（A-E）
  Phase 4: 资产图提示词（产品多视图、材质微距、品牌世界环境）
  Phase 5: 分镜关键帧提示词 + Seedance Multi-Phase 视频脚本
  Phase 6: 迭代优化
  Phase 7: 交付物整理
        ↓
  可直接复制使用的 Nano Banana Pro 提示词、
  Seedance 视频脚本和创意方案文档
```

## 入口模式

| 模式 | 触发信号 | 说明 |
|------|---------|------|
| **A：完整 TVC 创意流** | "帮我做一条xx产品广告" | Brief → 创意 → 画风 → 资产 → 分镜 → 打包 |
| **B：快速资产/提示词** | "帮我做一个产品 Hero Shot" | 跳过创意阶段，直接生成资产或关键帧提示词 |
| **C：分镜转化** | 提供 TVC 分镜脚本 | 画风 → 资产 → 将分镜转化为关键帧提示词 |
| **D：迭代修正** | "这张产品图xx不对" | 定位问题并提供修正版提示词 |

## TVC 叙事模型

| 模型 | 名称 | 核心逻辑 |
|------|------|---------|
| A | 痛点-解决 | 痛点场景 → 产品拯救 |
| B | 产品电影化拆解 | 多 Phase 微电影逐步揭示卖点 |
| C | 品牌世界穿梭 | 使用场景 ↔ 产品特写交叉剪辑 |
| D | 场景内叙事 | 产品始终在场景中，运镜突出 |
| E | 情感锚点 | 情感故事，产品为载体 |
| F | 蒙太奇揭示 | 视觉奇观 → 产品揭示 |
| G | 前后对比 | 使用前后的强烈反差 |
| H | 品牌宣言 | 价值观驱动，产品收束 |

## 交付物

```
my-tvc-project/
├── concept.md                      # TVC 创意方案文档
├── storyboard.md                   # 分镜脚本（如有）
│
├── assets/                         # 产品资产图提示词（Nano Banana Pro）
│   └── prompts/
│       ├── product-multiview.md
│       ├── product-detail-01.md
│       ├── env-01-extreme-sports.md
│       └── ...
│
├── keyframes/                      # 分镜关键帧提示词（Nano Banana Pro）
│   └── prompts/
│       ├── grid-01-brand-world.md
│       ├── grid-02-product-world.md
│       ├── endframe.md
│       └── ...
│
└── video-scripts/                  # Multi-Phase 视频提示词（Seedance）
    ├── segment-01-brand-world.md
    ├── segment-02-product-breakdown.md
    └── ...
```

## 如何使用交付物

1. **产品多视图** — 将 `assets/prompts/product-multiview.md` 中的提示词复制到 Nano Banana Pro，选择 edit 模式，传入参考图
2. **分镜关键帧** — 将 `keyframes/prompts/` 下的提示词复制到 Nano Banana Pro，edit 模式，传入多视图 + 环境图
3. **视频脚本** — 将 `video-scripts/` 下的 Multi-Phase 脚本配合多宫格首帧 + 产品多视图，输入 Seedance 生成视频

## 知识库架构

| 角色 | 文件 | 内容 | 加载时机 |
|------|------|------|---------|
| 核心流程 | `SKILL.md` | 入口判断、阶段流转、输出规范 | 始终加载 |
| 创意导演 | `treatment.md` | TVC 叙事模型、出镜策略、品类适配、视觉美学、创意方案模板 | 创意提案 |
| 镜头语言 | `shot-language.md` | 6 层提示词结构、画风锚定词库 A-E、12 种 TVC 场景类型、构图范式 | 视觉定调 / 前期筹备 / 分镜与拍摄 |
| 分镜与视频 | `storyboard.md` | 多宫格分镜、视频提示词语法、产品电影化拆解、品牌世界镜头 | 分镜与拍摄 |
| 前期筹备 | `pre-production.md` | 资产规划、生成顺序、各类资产标准、一致性维护 | 前期筹备 |
| 交付与迭代 | `delivery.md` | 输出格式模板、迭代调试指南（11 种常见失败模式） | 审片 / 交付 |

## License

MIT
