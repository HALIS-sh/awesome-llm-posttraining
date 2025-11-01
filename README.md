# Awesome-LLM-Post-training-Evaluation
Curated papers on LLM post-training (SFT→RL/RLVR): theory and mechanisms, training dynamics, evaluation/diagnostics, and cognition—each with a one-sentence summary plus links to PDF/code.

## 📚 Theory & Dynamics

- **RL’s Razor: Why Online Reinforcement Learning Forgets Less**（arXiv, 2025）  
  [PDF](https://arxiv.org/pdf/2509.04259) · — 在匹配新任务性能时，RL 相比 SFT 更少遗忘；核心因子是与基模型在新任务分布上的 KL 偏移，RL 天生偏向 KL 最小解。`tags: rl, sft, forgetting, kl, theory`

- **On Predictability of Reinforcement Learning Dynamics for Large Language Models**（arXiv, 2025）  
  [PDF](https://arxiv.org/pdf/2510.00553) · — 发现 RL 诱导的更新呈“秩-1 主导 / 线性动力学”，据此提出 AlphaRL，短窗外推即可加速训练并保持性能。`tags: rl, dynamics, rank1, acceleration, theory`

- **How Reinforcement Learning After Next-Token Prediction Facilitates Learning**（arXiv, 2025）  
  [PDF](https://arxiv.org/pdf/2510.11495) · — 给出框架解释为何“预训练(下一个词)→RL”能在推理任务中更高效学习，并展示 RL 增加测试时计算、拉长 CoT 的作用。`tags: rl, ntp, reasoning, cot, theory`

## 🧪 Pipeline & Diagnostics

- **Quagmires in SFT-RL Post-Training: When High SFT Scores Mislead and What to Use Instead**（arXiv, 2025）  
  [PDF](https://arxiv.org/pdf/2510.01624) · — 高 SFT 分数并不可靠预测 RL 之后表现；提出“泛化损失”“大 k 的 Pass@k”等更稳健代理指标；含大量对照实验与实务建议。`tags: sft, rlvr, metrics, diagnostics, pipeline`

## 🧠 Cognition & Test-time

- **Cognitive Behaviors that Enable Self-Improving Reasoners**（arXiv, 2025）  
  [PDF](https://arxiv.org/pdf/2503.01307v1) · — 识别四种有助自我改进的“认知行为”（验证、回溯、子目标、反向链），并用对照显示模型间差异与可迁移性。`tags: cognition, reasoning, behaviors, test-time`
