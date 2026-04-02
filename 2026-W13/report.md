# 具身智能一周动态｜第13周综合报告

> **数据范围**：2026年3月26日 — 4月2日
> **数据来源**：arXiv API + GitHub Trending/Search API
> **产出时间**：2026年4月2日

---

## 📖 一周导读

欢迎阅读第13周具身智能动态综合报告。本周是 VLA 架构井喷的一个星期，9篇 VLA 论文从不同维度突破，加上 **GENESIS** 以 28.4k⭐ 刷新仿真平台热度，具身智能正从"能做什么"向"怎么做更好"快速迭代。

### 🔍 快速导航

| 章节 | 内容 | 适合人群 |
|------|------|---------|
| **[一、本周数据总览](#一本周数据总览)** | 统计数据表格、论文/仓库分布图 | 快速了解全貌 |
| **[二、arXiv 论文精选](#二arxiv-论文精选)** | 7方向31篇论文详细整理 | 深入研究 |
| **[三、GitHub 开源项目](#三github-开源项目)** | 新建仓库+经典仓库精选 | 找代码/工具 |
| **[四、本周核心洞察](#四本周核心洞察)** | 大趋势+子方向动态 | 把握方向 |

### ⚡ 本周一句话速览

| 维度 | 最大新闻 |
|------|---------|
| **论文** | VLA 领域 5大架构方向同时突破（DIAL/FocusVLA/DFM-VLA/Fast-dVLA/MMaDA-VLA） |
| **开源** | GENESIS 28.4k⭐ 开创生成式仿真新范式 |
| **硬件** | 人形机器人（Unitree G1）+被动弹性关节四足成为数据效率研究载体 |
| **方法** | 扩散策略从生成扩散→动作细化→世界模型，全链路渗透 |
| **安全** | 具身AI安全综述（400+论文）+ VLM affordance gap 实证研究双双出现 |

---

## 一、本周数据总览

### 1.1 论文统计

| 方向 | 论文数 | 占总量比 | 核心关键词 |
|------|--------|---------|-----------|
| 🧩 VLA（具身智能体与大模型） | **9篇** | 29.0% | DIAL、FocusVLA、DFM-VLA、Fast-dVLA、MMaDA-VLA |
| 🤖 具身控制与操作 | **9篇** | 29.0% | 扩散策略、模仿学习、灵巧手、人形 |
| 🗺️ 具身决策与规划 | **5篇** | 16.1% | LLM规划、MILP-MPC、逆动力学谱分解 |
| 🤝 人机交互 | **5篇** | 16.1% | 隐式控制、VR遥现、知识图谱、共享autonomy |
| 🌍 世界模型与强化学习 | **4篇** | 12.9% | HCLSM、LOME、Persistent WM、OmniVTA |
| 🧠 具身感知 | **2篇** | 6.5% | VLM affordance limits、OVI-MAP |
| 🧪 仿真、数据与平台 | **2篇** | 6.5% | V-Dreamer、Fire as a Service |

> 📌 注：部分论文因主题交叉可归入多个方向，合计31篇去重。

### 1.2 GitHub 仓库统计

| 方向 | 新建仓库 | 代表⭐ | 经典仓库代表 |
|------|---------|--------|------------|
| 🧪 仿真、数据与平台 | **4个** | GENESIS 28.4k | Awesome-World-Model 1.9k |
| 🤝 人机交互 | **7个** | Smalltalk-KG 1⭐ | — |
| 🌍 世界模型与RL | **8个** | Awesome-Embodied-AI-Safety 50 | DreamerV2 1k、TDMPC2 780 |
| 🤖 具身控制与操作 | **4个** | ComfyUI-Kimodo 18 | RDT-1B 1.7k、DIAL-MPC 953 |
| 🧩 VLA | **0个**新建 | — | GigaBrain-0 2.5k、VLA-Adapter 2.1k |
| 🗺️ 具身决策与规划 | **2个** | RoboWrist 0⭐ | DreamDojo 679 |
| 🧠 具身感知 | **2个** | — | DID-Safety-System 0⭐ |

### 1.3 论文发表时间分布

| 发布日期 | 篇数 | 代表作 |
|---------|------|--------|
| 4月2日 | 3 | DreamControl-v2、MILP-MPC导航 |
| 3月31日 | 4 | DIAL、HCLSM、Hybrid RL+LLM、WoZ Interface |
| 3月30日 | 5 | TAG触觉手套、Active Stereo、人形学习、StretchBot |
| 3月29日 | 4 | ProgressVLA、被动滚轮指尖、FlowRL、神经形态 |
| 3月28日 | 0 | — |
| 3月27日 | 5 | VLM Limits、OVI-MAP、MuscleMimic、VLA-OPD、Realtime-VLA |
| 3月26日 | 4 | PoE负反馈、Persistent WM、Fast-dVLA、VideoWeaver |

### 1.4 关键数据可视化概览（见 HTML 版）

> 以下数据请查看 HTML 报告中的交互式图表：
> - **图1**：7方向论文数量分布（饼图）
> - **图2**：arXiv 论文每日发表趋势（柱状图）
> - **图3**：GitHub 经典仓库星标对比（条形图）
> - **图4**：本周技术热词词云（由 arXiv 标题词频生成）

---

## 二、arXiv 论文精选

---

### 📌 方向一：具身感知与场景理解（2篇）

> 本周共 2 篇，主要聚焦 VLM 具身缺陷实证和零样本语义建图。

| # | 论文 | arXiv ID | 一句话贡献 | 亮点 |
|---|------|----------|-----------|------|
| 1 | **The Limits of Learning from Pictures and Text** | 2603.26589 | 对比18个VLM与2000+人类，揭示VLM在affordance任务上存在**结构性缺陷**，缺乏具身经验是根本原因 | ⭐ 必读 |
| 2 | **OVI-MAP** | 2603.26541 | 3D实例重建与语义推理解耦，VLM零样本开放词汇建图，实时优于SOTA | 零样本 |

**🔑 关键洞察**：两篇论文形成"批判VLM→改进建图"的呼应，揭示视觉-语言模型在具身场景的结构性局限，同时给出解决路径。

---

### 📌 方向二：具身决策与规划（5篇）

> 本周共 5 篇，覆盖 LLM规划、几何感知导航、逆动力学等方向。

| # | 论文 | arXiv ID | 一句话贡献 | 亮点 |
|---|------|----------|-----------|------|
| 1 | **DreamControl-v2** | 2604.00202 | 在人形运动空间训练引导扩散先验，多样化数据聚合到统一具身空间，解决长时程规划 | ⭐ 人形 |
| 2 | **MILP-MPC + CBFs 多面体导航** | 2604.00162 | MILP + Minkowski差空间CBF，实现非凸环境长时程安全导航 | 安全 |
| 3 | **Hybrid RL+LLM** | 2603.30022 | LLM高层规划 + RL低层控制，Franka Panda验证性能提升 | 混合 |
| 4 | **osmAG-Nav** | 2603.28271 | 开源ROS2分层语义拓扑导航栈，多楼层长期定位 | ⭐ 开源 |
| 5 | **逆动力学谱分解** | 2603.27796 | 谱分解搜索树，接触密集场景实时长时程规划 | 新方法 |

---

### 📌 方向三：具身控制与操作（9篇）— 热门方向

> 本周最热方向之一，涵盖能量高效运动、触觉手套、多视角模仿学习等。

| # | 论文 | arXiv ID | 一句话贡献 | 亮点 |
|---|------|----------|-----------|------|
| 1 | **PIL四足能量高效运动** | 2604.00611 | RL策略蒸馏到被动弹性关节（PEJ），平地87%机械功率卸载 | 硬件协同 |
| 2 | **Multi-Camera View Scaling** | 2604.00557 | 多相机同步视角生成伪示范，数据效率和视角泛化双提升 | ⭐ 数据效率 |
| 3 | **TAG触觉反馈手套** | 2603.28542 | 21-DoF磁感手势捕捉 + 32致动器/指触觉阵列，触觉在环遥操作 | 硬件 |
| 4 | **Active Stereo > Multi-Sensor** | 2603.28422 | Unitree G1上14种传感器组合评测，简单主动双目87.5%胜出 | ⭐ 反直觉 |
| 5 | **ProgressVLA** | 2603.27670 | 进度估计+逆动力学世界模型，解决VLA长程自适应终止问题 | VLA+ |
| 6 | **被动滚轮指尖** | 2603.27452 | 被动滚轮可调制摩擦和约束方向，使标准爪手实现滑动/枢转 | 硬件 |
| 7 | **FlowRL** | 2603.27450 | 扩散策略RL系统性分类学，模块化JAX开源基准 | ⭐ 基准 |
| 8 | **PoE负反馈模仿学习** | 2603.26467 | 从次优示范和失败中学习，模糊任务成功率+90% | 容错 |
| 9 | **MuscleMimic** | 2603.25544 | 126~416肌肉GPU并行仿真，策略在真实肌肉控制下复现人类运动 | ⭐ 规模 |

**🔑 关键洞察**：人形/四足+软体硬件（PEJ/被动滚轮/触觉阵列）与学习算法协同优化成为新范式；Active Stereo 胜过多传感器是本周最反直觉发现。

---

### 📌 方向四：具身强化学习与世界模型（4篇）

> 本周 4 篇，世界模型实用化趋势明确。

| # | 论文 | arXiv ID | 一句话贡献 | 亮点 |
|---|------|----------|-----------|------|
| 1 | **HCLSM** | 2603.29090 | 物体分解+分层因果+结构学习，PushT上低MSE预测 | 因果 |
| 2 | **LOME** | 2603.27449 | 自我中心视频世界模型，文本+人体动作→人-物交互视频 | AR/VR |
| 3 | **Persistent Robot WM** | 2603.25685 | RL后训练解决多步rollout误差累积问题 | 稳定性 |
| 4 | **OmniVTA** | 2603.19201 | 视触觉世界模型+60Hz反射控制器，未见物体强泛化 | ⭐ 触觉 |

**🔑 关键洞察**：视触觉+世界模型成为新组合（LOME、OmniVTA）；RL后训练（Persistent WM）解决世界模型部署难题。

---

### 📌 方向五：VLA（9篇）— ⭐本周最热方向

> 9 篇 VLA 论文覆盖架构创新、后训练、推理优化三大类。

| # | 论文 | arXiv ID | 一句话贡献 | 亮点 |
|---|------|----------|-----------|------|
| 1 | **DIAL** | 2603.29844 | 🌟 System-2潜在世界建模 + System-1动作解码，10x少示范达到SOTA | ⭐⭐ 必读 |
| 2 | **FocusVLA** | 2603.28740 | 🌟 揭示VLA瓶颈在视觉信息利用方式，模态级联+焦点注意力 | ⭐⭐ 必读 |
| 3 | **LIBERO-Para** | 2603.28301 | 首个VLA指令改写鲁棒性基准，22~52pp性能下降，80~96%失败源于规划 | 基准 |
| 4 | **VLA-OPD** | 2603.26666 | 专家蒸馏+反向KL目标，RL效率+SFT鲁棒性兼得 | 后训练 |
| 5 | **Realtime-VLA V2** | 2603.26360 | VLA高速运行实用技术栈，逼近人类操作速度 | 部署 |
| 6 | **DFM-VLA** | 2603.26320 | 离散流匹配迭代动作细化，LIBERO 95.7%成功率 | 动作细化 |
| 7 | **Fast-dVLA** | 2603.25661 | 参数空间辅助目标解耦，标准SFT简洁实现辅助训练增强 | 加速 |
| 8 | **VideoWeaver** | 2603.25420 | 首个多视角V2V翻译，支持ego和异构相机设置一致性 | V2V |
| 9 | **MMaDA-VLA** | 2603.25406 | 统一离散扩散VLA，LIBERO 98.0%，CALVIN 4.78 | ⭐ SOTA |

**🔑 关键洞察**：DIAL 和 FocusVLA 揭示VLA从"堆参数"向"架构设计"转型；MMaDA-VLA统一扩散+VLA刷新SOTA；LIBERO-Para揭示指令改写是VLA落地的关键瓶颈。

---

### 📌 方向六：仿真、数据与平台（2篇）

| # | 论文 | arXiv ID | 一句话贡献 | 亮点 |
|---|------|----------|-----------|------|
| 1 | **V-Dreamer** | 2603.18811 | LLM+3D生成全自动仿真场景，视频运动先验合成可执行轨迹 | Sim-to-Real |
| 2 | **Fire as a Service** | 2603.19063 | 高保真火灾热力学仿真+体积烟雾，支持消防机器人遥操作训练 | 垂直场景 |

---

### 📌 方向七：人机交互与具身社会智能（5篇）

| # | 论文 | arXiv ID | 一句话贡献 | 亮点 |
|---|------|----------|-----------|------|
| 1 | **StretchBot** | 2604.00628 | 知识图谱+LLM自适应辅助拉伸/康复指导 | 知识图谱 |
| 2 | **WoZ Interface Choices** | 2603.28338 | VR遥现界面在用户偏好和社会存在感上均最优 | VR |
| 3 | **Implicit Control** | 2603.28079 | 基于自然行为线索的隐式控制范式，保留用户控制感 | ⭐ 新范式 |
| 4 | **最小能耗pHRI** | 2603.25259 | 移动操作臂最小动能控制器 | 能耗 |
| 5 | **DiSCo** | 2603.22787 | 扩散策略+共享autonomy，驾驶和机械臂任务显著提效 | 共享autonomy |

---

## 三、GitHub 开源项目

---

### 🏆 本周 GitHub Top 3

| 排名 | 仓库 | ⭐ | 方向 | 入选理由 |
|------|------|-----|------|---------|
| 🥇 | **GENESIS-EMBODIED-AI/GENESIS** | 28.4k | 仿真平台 | 本周全领域最热，生成式具身AI学习世界 |
| 🥈 | **x-zheng16/Awesome-Embodied-AI-Safety** | 50 | 安全 | 400+论文安全综述，填补领域空白 |
| 🥉 | **jtydhr88/ComfyUI-Kimodo** | 18 | 具身控制 | NVIDIA Kimodo运动扩散模型集成 |

---

### 3.1 新建仓库精选（本周创建）

| 方向 | 仓库 | ⭐ | 语言 | 亮点 |
|------|------|-----|------|------|
| 🧪 仿真 | **GENESIS-EMBODIED-AI/GENESIS** | 28.4k | — | ⭐⭐⭐ 本周最热，生成式具身AI世界 |
| 🌍 世界模型 | **x-zheng16/Awesome-Embodied-AI-Safety** | 50 | — | 具身AI安全综述400+论文 |
| 🤖 具身控制 | **jtydhr88/ComfyUI-Kimodo** | 18 | Python | NVIDIA Kimodo运动扩散集成 |
| 🌍 世界模型 | **0xNickdev/neurolobster** | 26 | Python | 神经形态具身仿真（真实神经动力学驱动） |
| 🤝 HRI | **hcr-lab/Smalltalk-KG** | 1 | Python | 知识图谱+长期对话记忆HRI框架 |
| 🤝 HRI | **ninja-otaku/neuropose** | 1 | Python | 人体姿态→机器人运动（零成本遥操作） |
| 🌍 世界模型 | **apolloil/Embodied-RL-Post-Training** | 1 | Python | GPT Policy + C51的MetaWorld RL后训练 |
| 🤖 具身控制 | **terryum/book-robot-hand-tactile-sensor** | 1 | TeX | 灵巧手触觉传感综述 |

---

### 3.2 经典仓库更新（高影响力持续活跃）

#### VLA 生态（方向五）

| 仓库 | ⭐ | 描述 |
|------|-----|------|
| **JonyZhang2023/AWESOME-EMBODIED-VLA-VA-VLN** | 2.9k | 具身AI/VLA/VLN最新研究精选列表 |
| **OPEN-GIGAAI/GIGA-BRAIN-0** | 2.5k | 世界模型驱动的视觉-语言-动作模型 |
| **OPENHELIX-TEAM/VLA-ADAPTER** | 2.1k | 小规模VLA高效微调范式 |
| **SHOWLAB/SHOWUI** | 1.8k | [CVPR 2025] 开源端到端VLA用于GUI智能体 |
| **STARVLA/STARVLA** | 1.5k | 乐高式VLA开发代码库 |
| **AllenzRen/OPEN-PI-ZERO** | 1.4k | Physical Intelligence pi0 VLA复现 |
| **DEXMAL/DEXBOTIC** | 890 | 开源VLA工具箱 |
| **SPATIALVLA/SPATIALVLA** | 676 | 110万真实机器人片段训练的空间增强VLA |

#### 扩散策略+具身控制（方向三）

| 仓库 | ⭐ | 描述 |
|------|-----|------|
| **THU-ML/RoboticsDiffusionTransformer** | 1.7k | RDT-1B：双臂操作扩散基础模型 |
| **LECAR-Lab/DIAL-MPC** | 953 | 扩散风格退火MPC（人形足式控制） |
| **DYSON-AI/HDP** | 231 | [CVPR 2024] 分层扩散策略多任务操作 |
| **WEIRDLabUW/unified-world-model** | 202 | 视频+动作扩散统一世界模型 |
| **lucidrains/diffusion-policy** | 134 | Diffusion Policy Toyota Research实现 |

#### 世界模型（方向四）

| 仓库 | ⭐ | 描述 |
|------|-----|------|
| **DANIJAR/DREAMERV2** | 1k | DreamerV2: 离散世界模型掌握Atari |
| **ROBBYANT/LINGBOT-VA** | 942 | 因果视频-动作世界模型 |
| **THU-ML/MOTUS** | 923 | Motus: 统一潜动作世界模型 |
| **NICKLASHANSEN/TDMPC2** | 780 | TD-MPC2: 可扩展鲁棒世界模型连续控制 |
| **LEGGEDROBOTICS/robotic_world_model** | 559 | 机器人世界模型+不确定性感知 |
| **1X-TECHNOLOGIES/1XGPT** | 557 | 人形机器人世界建模挑战赛 |

---

## 四、本周核心洞察

### 4.1 五大核心趋势

#### 🔥 趋势一：VLA 架构从"暴力扩展"转向"精细设计"

本周 9 篇 VLA 论文的核心洞察：**DIAL** 通过 System-2/1 解耦实现 10x 数据效率，**FocusVLA** 揭示瓶颈在视觉利用而非表征，**Fast-dVLA** 用参数差值替代辅助损失。这三篇论文共同指向一个方向：VLA 的下一波突破来自**架构设计**，而非简单增大模型。

#### 🔥 趋势二：扩散策略全链路渗透

从动作生成（RDT-1B、DFM-VLA）→ 运动先验（ComfyUI-Kimodo）→ 世界模型（unified-world-model）→ 共享autonomy（DiSCo）→ 模仿学习（FlowRL taxonomy），扩散模型已成为具身智能的"通用语言"。

#### 🔥 趋势三：具身 AI 安全从隐到显

- **arxiv**：VLM affordance gap 实证研究（"Limits of VLM"）
- **GitHub**：Awesome-Embodied-AI-Safety（400+论文）、DREAMDOJO-AEGIS-SDK

#### 🔥 趋势四：人形机器人成为"数据效率"研究主战场

Unitree G1（Active Stereo实验）、Figure/Stanford GR1（DIAL零样本泛化）、Tesla Optimus 相关研究共同指向：人形机器人因为形态通用性，成为验证数据高效方法（少样本、零样本、跨任务）的最佳载体。

#### 🔥 趋势五：触觉+世界模型成为新组合

OmniVTA（视触觉世界模型）、TAG（触觉反馈手套）、Neurolobster（神经形态具身）三者均指向"多模态感知→世界模型→精细控制"的闭环，触觉传感正在从"附加传感器"升级为"核心模态"。

### 4.2 开放问题与待关注方向

| 问题 | 来源 | 为什么重要 |
|------|------|----------|
| VLA 指令改写鲁棒性 | LIBERO-Para：22~52pp性能下降 | 直接影响真实场景部署 |
| 触觉在数据有限regime下成为噪声 | Active Stereo实验 | 与直觉相反，值得深入研究 |
| VLM affordance gap | "Limits of VLM"论文 | 视频/文本数据无法解决的结构性问题 |
| 扩散策略RL训练稳定性 | FlowRL taxonomy | 需要系统性工程方案 |

### 4.3 下周值得关注

1. **DIAL 复现进展**：System-2/1 解耦范式可能引发一波跟进工作
2. **GENESIS 实际性能**：28.4k⭐的生成式仿真平台能否兑现承诺值得关注
3. **Awesome-Embodied-AI-Safety**：安全综述可能催生安全导向的具身智能研究社区
4. **Neurolobster 神经形态路线**：真实神经动力学驱动机器人 vs 深度学习逼近，谁更有前景？

---

## 📎 附录

### A. 论文索引表

| 方向 | arXiv ID | 论文简称 |
|------|----------|---------|
| 感知 | 2603.26589 | Limits of VLM |
| 感知 | 2603.26541 | OVI-MAP |
| 决策 | 2604.00202 | DreamControl-v2 |
| 决策 | 2604.00162 | MILP-MPC导航 |
| 决策 | 2603.30022 | Hybrid RL+LLM |
| 决策 | 2603.28271 | osmAG-Nav |
| 决策 | 2603.27796 | 逆动力学谱分解 |
| 控制 | 2604.00611 | PIL四足 |
| 控制 | 2604.00557 | Multi-Camera Scaling |
| 控制 | 2603.28542 | TAG触觉手套 |
| 控制 | 2603.28422 | Active Stereo人形 |
| 控制 | 2603.27670 | ProgressVLA |
| 控制 | 2603.27452 | 被动滚轮指尖 |
| 控制 | 2603.27450 | FlowRL |
| 控制 | 2603.26467 | PoE负反馈 |
| 控制 | 2603.25544 | MuscleMimic |
| 世界模型 | 2603.29090 | HCLSM |
| 世界模型 | 2603.27449 | LOME |
| 世界模型 | 2603.25685 | Persistent Robot WM |
| 世界模型 | 2603.19201 | OmniVTA |
| VLA | 2603.29844 | DIAL |
| VLA | 2603.28740 | FocusVLA |
| VLA | 2603.28301 | LIBERO-Para |
| VLA | 2603.26666 | VLA-OPD |
| VLA | 2603.26360 | Realtime-VLA V2 |
| VLA | 2603.26320 | DFM-VLA |
| VLA | 2603.25661 | Fast-dVLA |
| VLA | 2603.25420 | VideoWeaver |
| VLA | 2603.25406 | MMaDA-VLA |
| 仿真 | 2603.18811 | V-Dreamer |
| 仿真 | 2603.19063 | Fire as a Service |
| HRI | 2604.00628 | StretchBot |
| HRI | 2603.28338 | WoZ Interface |
| HRI | 2603.28079 | Implicit Control |
| HRI | 2603.25259 | 最小能耗pHRI |
| HRI | 2603.22787 | DiSCo |

---

*本报告由 WorkBuddy 自动生成 | arxiv-watcher + github-trending skill 联合驱动*
*数据来源：arXiv API（31篇论文）+ GitHub API/Search（30+仓库）*
*生成时间：2026-04-02*
