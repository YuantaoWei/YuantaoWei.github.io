---
title: "Projects"
permalink: /projects/
---

My research focuses on causal discovery and inference, probabilistic machine learning, and LLM-based decision-making. At the University of Washington, I work with Prof. Shuai Huang on methods that learn from human knowledge, reason under uncertainty, and connect causal models with practical decisions.

## Research Projects

### Mixture-of-Chains: Causal Discovery from Human Knowledge

*Accepted at NeurIPS 2026 · Co-first author*

How can expert judgments be translated into a coherent causal graph? I developed **Mixture-of-Chains (MoC)**, a framework that represents expert knowledge through a mixture of latent causal chains and recovers a directed acyclic graph (DAG).

- **Method:** Combined latent chain discovery, aggregation, and DAG decoding in a multi-stage framework to recover causal structure directly from expert knowledge.
- **Results:** Reduced structural Hamming distance (SHD, a measure of graph-recovery error) by **29% on average** across five networks and four ranking-based baselines, with a **46% reduction relative to the strongest baseline**.
- **Further evaluation:** Used MoC-derived priors in observational causal discovery and improved graph recovery.

### Bayesian DAG-IRT: Modeling Expert Ability and Judgment Difficulty

*Under review at AISTATS 2027 · Co-first author*

Expert judgments vary in reliability, and some causal relationships are harder to assess than others. I developed **DAG-IRT**, a Bayesian item response framework that models these differences when aggregating judgments into a causal graph.

- **Method:** Jointly inferred graph structure, expert ability, and judgment difficulty, while quantifying posterior uncertainty over the recovered graph.
- **Results:** Outperformed all evaluated crowdsourcing baselines across **four synthetic benchmark networks and two human-judgment tasks**. Achieved **27% lower SHD on average** than the evaluated baselines, including majority voting and Dawid-Skene.

### Kernel Residual Displacement: Causal Discovery under Distribution Shifts

*Under review at ICLR 2027*

Operational shifts change how a system behaves. In this project, I investigated how observations from **two regimes** can help identify causal direction between two variables using **kernel residual displacement (KRD)**.

- **Theory:** Studied identifiability and finite-sample guarantees under the study's assumptions.
- **Results:** KRD averaged **10.8 percentage points higher accuracy** than nine baselines across eight real-data tasks.

Related paper: *The System Is Out of Control, but Causality Isn't: Leveraging Operational Shifts for Bivariate Causal Discovery.*

### TwinPlan: LLM Agents and Digital Twins for Health Planning

*Under review at KDD 2027*

I contributed to **TwinPlan**, an LLM-agent and digital-twin framework for personalized health planning. The framework translates plans into executable interventions and compares them through counterfactual simulation.

- **Approach:** Connected LLM-based planning with digital-twin simulation to evaluate candidate interventions.
- **Results:** On **100 semi-synthetic cases**, the framework achieved **Set F1 of 0.900**, a **41% average gain across three baseline families** and **22% above the strongest baseline**, with **100% decision coverage**.

### Digital Twins for Food Supply Chains

*Ongoing research*

I am developing a digital-twin framework for **last-mile cold-chain delivery** that couples food-quality dynamics with logistics decisions.

- **Modeling focus:** Represent how food quality evolves alongside delivery operations.
- **Decision focus:** Study adaptive decisions through sequential twin-state updates, considering trade-offs among shelf life, transportation cost, and food waste.

## Industry Projects

### Quantitative Strategy Backtesting

*Foresight Fund Management Company · Quantitative Research Intern · March-August 2024*

Replicated and refined A-share strategies, including equal-weight rebalancing and Quant-Minus-Junk variants. Built a systematic backtesting framework and analyzed discrepancies between backtest and live-market performance.

### Data Pipelines and Generative-AI Applications

*Deloitte · Data Analysis Intern · September-December 2023*

Built Python pipelines for data collection, cleaning, and integration to support model-training workflows for an intelligent data platform. Assisted with model testing, prompt tuning, and deployment validation for LLM and multimodal-generation applications.

### Sound-Scene Classification for Cochlear Implants

*MicroPort Medical · Algorithm Intern · July-September 2023*

Developed a CNN-based classification workflow using **40,000+ audio samples**. Improved accuracy from **60% to 85% (+25 percentage points)** through architecture optimization and test refactoring. Prepared technical documentation and supported patent-material preparation.

## Technical Toolkit

- **Programming:** Python, SQL, R
- **Machine learning:** PyTorch, TensorFlow, scikit-learn
- **Causal modeling:** causal-learn, pgmpy, DoWhy, gCastle
- **Research tools:** Git, GitHub, LaTeX, cloud computing
