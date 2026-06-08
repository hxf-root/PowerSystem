# PowerSystem

> 电力系统理论学习 · 费曼检验 · 代码落地

从一个 FTU / 嵌入式工程师的视角，系统学习电力系统理论。目标不是"看懂教材"，而是把原理讲清楚、写出能跑的代码。

---

## 路线

学习体系分为八层，逐层递进：

| # | 层 | 状态 |
|---|-----|------|
| 0 | **数学工具** — 相量 / 对称分量法 / 标幺制 | ✅ 已完成 |
| 1 | **物理本质** — 电压 / 电流 / 功率 | ✅ 已完成 |
| 2 | **测量系统** — CT / PT / 采样算法 | ✅ 已完成 |
| 3 | **三相交流系统** — 对称分量 / 中性点接地 | ✅ 已完成 |
| 4 | **电网结构** — 发输变配用 / 配网拓扑 | ✅ 已完成 |
| 5 | **系统分析** — 潮流 / 短路 / 稳定性 | ✅ 已完成 |
| 6 | **继电保护** — 过流 / 零序 / 方向 / 差动 | ✅ 已完成 |
| 7 | **配电自动化** — FA / FTU / 104 规约 | 🚧 进行中 |

详细路线图参见 [路线.md](路线.md)。

---

## 当前进度

第一阶段（第 0~3 层）和第二阶段的第 4~6 层已完成，已经开始第 7 层——配电自动化（FA、FTU、104 规约）。

| 文件 | 内容 |
|------|------|
| [第0层-数学工具.md](第0层-数学工具.md) | 相量、对称分量法（数学）、标幺制 |
| [第1层-物理本质.md](第1层-物理本质.md) | 电压、电流、功率（有功/无功/视在） |
| [第2层-测量系统.md](第2层-测量系统.md) | CT、PT、接线方式、误差链、电量计算 |
| [第3层-三相交流系统.md](第3层-三相交流系统.md) | 对称分量（物理意义）、中性点接地、相序 |
| [第4层-电网结构.md](第4层-电网结构.md) | 发输变配用、电压等级分层、配网拓扑、接地方式选型 |
| [第5层-系统分析.md](第5层-系统分析.md) | 潮流、短路、稳定性、系统分析与 FTU 连接 |
| [第6层-继电保护.md](第6层-继电保护.md) | 保护四性、过流、零序、方向、差动、配电保护特点 |
| [第7层-配电自动化.md](第7层-配电自动化.md) | FA、FTU、三遥、IEC104 / 61850、拓扑恢复 |

### 动画资源（SVG，共 25 张）

---

## 学习方法

```
  理论 ←──→ 工程 ←──→ 代码
```

每个知识点从三个维度展开：

| 维度 | 说明 |
|------|------|
| **理论** | 物理原理和数学推导，讲清楚"为什么" |
| **工程** | 对应什么现场现象、FTU 的什么功能 |
| **代码** | 如何用代码表达这个原理 |

每层末尾有 **费曼检验** — 用自己的话讲清楚核心概念，才算过关。

---

## 文件结构

```
PowerSystem/
├── README.md
├── 路线.md
├── 欢迎.md
├── 第0层-数学工具.md
├── 第1层-物理本质.md
├── 第2层-测量系统.md
├── 第3层-三相交流系统.md
├── 第4层-电网结构.md
├── 第5层-系统分析.md
├── 第6层-继电保护.md
└── assets/
    ├── phasor-rotation.svg
    ├── generator-coil.svg
    ├── slip-ring-brush.svg
    ├── ct-principle.svg
    ├── ct-saturation-waveform.svg
    ├── pt-principle.svg
    ├── pt-vv-wiring.svg
    ├── pt-yy-wiring.svg
    ├── pt-open-delta.svg
    ├── error-chain.svg
    ├── three-phase-waveform.svg
    ├── symmetrical-components-decomposition.svg
    ├── neutral-grounding-comparison.svg
    ├── power-grid-structure.svg
    ├── distribution-topology.svg
    ├── voltage-hierarchy.svg
    ├── power-flow-study.svg
    ├── system-analysis-overview.svg
    ├── short-circuit-study.svg
    ├── stability-swing.svg
    ├── protection-overview.svg
    ├── protection-coordination.svg
    ├── fa-restoration-flow.svg
    ├── ftu-functional-architecture.svg
    └── communication-protocols.svg
```

---

## 参考

- [www.pengky.cn](https://www.pengky.cn) — 电机系列动画
- 电力系统分析（教材）
- 国家电网公司继电保护规程
