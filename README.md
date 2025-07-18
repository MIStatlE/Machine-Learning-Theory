# 📚 机器学习理论 · 资源库

面向希望**系统性攻读机器学习理论**（Machine Learning Theory, MLT）的同学，整理了常用教材、课程笔记、优质网课，以及推荐的先修要求与学习顺序，帮助快速构建完整的知识图谱。

> **如何使用：**  
> 1. 按“学习路径总览”循序渐进；  
> 2. 在每门课的 *Books / Notes / MOOCs* 栏挑选资源；  
> 3. 配合“作用说明”理解该课在 MLT 中的定位；  
> 4. 欢迎 PR 更新、补充与纠错 🚀。

---

## 🗺️ 学习路径总览

| 阶段 | 建议课程 | 目标与能力 |
|------|----------|------------|
| **Ⅰ. 数学基础** | 线性代数 → 概率统计 → 实分析 ➕ 优化理论 | 搭建分析与证明工具箱 |
| **Ⅱ. 核心理论** | 统计学习理论 → 高维概率 → 凸优化与对偶 → 泛化与复杂度 | 掌握 PAC/VC、Rademacher、信息论等关键框架 |
| **Ⅲ. 高级专题** | 强化学习理论 → 在线/Bandit 学习 → 深度学习理论 | 站在前沿阅读顶会 / 论文，理解开放问题 |
| **Ⅳ. 研究实践** | 研读 COLT / NeurIPS / ICML 理论论文 | 能独立追踪 & 评价最新进展 |

---

## 📖 课程资源

### Ⅰ. 数学基础 <a id="数学基础"></a>

| 课程 | Books | Notes / Slides | MOOCs | Prerequisite | 在 MLT 中的作用 |
|------|-------|----------------|-------|--------------|-----------------|
| **线性代数** | *Matrix Analysis* — Horn & Johnson；*Linear Algebra Done Right* — Axler | MIT 18.06 笔记 | MIT OpenCourseWare 18.06；3Blue1Brown *Essence of LA* | 高中数学 | 向量空间、特征分解、奇异值是泛化与优化分析的基石 |
| **概率论与统计** | *Probability Theory* — Gut；*Statistical Inference* — Casella & Berger | CMU 36-705 讲义 | Harvard *Stat 110* | 微积分 | 建立随机变量、极限定理直觉，为泛化与上界/下界奠基 |
| **实分析** | *Principles of Mathematical Analysis* — Rudin | MIT 18.100B 手写笔记 | - | 微积分 | 掌握极限、测度，支撑严谨证明（如可测性假设） |
| **凸优化** | *Convex Optimization* — Boyd & Vandenberghe | Stanford EE364A 讲义 | Stanford *EE364A* (YouTube) | 线性代数 | 学习损失最小化、本征维等算法分析框架 |

---

### Ⅱ. 核心理论 <a id="核心理论"></a>

| 课程 | Books | Notes / Slides | MOOCs | Prerequisite | 在 MLT 中的作用 |
|------|-------|----------------|-------|--------------|-----------------|
| **统计学习理论 (SLT)** | *Understanding Machine Learning* — Shalev-Shwartz & Ben-David | 讲义 by Shalev-Shwartz (Hebrew U.) | Y. Singer *Statistical Learning* (Coursera) | 概率论、凸优化 | AVC 维、Uniform Convergence、PAC Bayes 等核心概念 |
| **高维概率** | *High-Dimensional Probability* — Vershynin | ETH 课程笔记 | Roman Vershynin 视频课程 | 概率论、线代 | 支撑随机矩阵、集中不等式分析 |
| **泛化与复杂度** | *Foundations of ML* — Mohri, Rostamizadeh, Talwalkar (2e) | NYU DS-MLT 讲义 | - | SLT | Rademacher、Covering Numbers、算法依赖复杂度 |
| **信息论方法** | *Elements of Information Theory* — Cover & Thomas | Caltech EE126 讲义 | Caltech EE126 | 概率论 | 推导 minimax 下界、后验压缩 |

---

### Ⅲ. 高级专题 <a id="高级专题"></a>

| 课程 | Books / Surveys | Notes / Slides | MOOCs | Prerequisite | 在 MLT 中的作用 |
|------|-----------------|----------------|-------|--------------|-----------------|
| **强化学习理论 (RL Theory)** | *Reinforcement Learning: An Introduction* — Sutton & Barto；*Bandit Algorithms* — Lattimore & Szepesvári | UCL RL Theory 讲义 | David Silver *RL* (YouTube) | 马尔可夫过程、SLT | 研究采样效率、探索 vs. 利用、 regret 下界 |
| **在线 / Bandit 学习** | see *Bandit Algorithms* | COLT Short Course (Bubeck & Cesa-Bianchi) | - | 凸优化、高维概率 | 分析 adversarial / stochastic 场景中的决策效率 |
| **深度学习理论** | *Deep Learning Theory* (forthcoming notes)；survey by Moritz Hardt et al. | Stanford CS330 Notes | ApproxML *Deep Theory* Lectures | 高维概率、信息论 | 研究表示能力、优化景观、implicit bias |

---

## 🛠️ 贡献指南 <a id="贡献指南"></a>

1. **Fork → Clone → 新分支**。  
2. 在相应目录下新增或更新资源：  
   - `books/` 书籍 PDF / 购买链接  
   - `notes/` 个人或公开课程笔记  
   - `moocs/` 视频课程清单  
3. PR 标题格式：`[Add] 课程名 - 资源类型`。  
4. 通过 CI (`mdlint`) 确保格式无误。  

---

## 📜 License <a id="license"></a>

本仓库除特别说明外，均采用 **CC BY-NC-SA 4.0** 许可协议。商用或改编请注明出处。

---

> 🌟 **愿景**：构建华语世界最系统的机器学习理论学习路线图，让研究者与学习者能够“少走弯路，多做深入”。若本文档对你有帮助，请 star ⭐️ 支持！


> 每个子目录下包含  
> • 📚 **books/** – 官方 PDF/合法电子稿  
> • 📝 **notes/** – Markdown/Jupyter 笔记  
> • 🔗 **links.md** – 高质量外部资源索引  




