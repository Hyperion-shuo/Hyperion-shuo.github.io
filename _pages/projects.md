---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

## IEEE CoG2021 Fighting Game AI Competition (2021/6 - 2021/8)

- Won the championship of IEEE CoG2021 Fighting Game AI Competition, achieving **100% win rate** in both PVE speedrun and PVP three-character tracks.
- Developed a distributed Population-Based Training (PBT) framework for fighting games, enabling reward style parameters to converge to fixed values.

---

## IEEE CoG2022 Google Research Football Multi-Agent AI Competition (2022/5 - 2022/9)

- Analyzed top single-agent football solutions on Kaggle. Built features and rewards. Developed specific scenarios to enhance skills like kickoff, one-two passing, etc. Created models with different styles by designing various rewards.
- Innovated a hybrid opponent pool sampling mechanism, integrating multiple algorithms and model types. Implemented large-scale distributed PPO model training.
- Designed a multi-stage model selection process: initial Elo screening, specific scenario skill evaluation, comprehensive style assessment (goals, shots, possession, interceptions), and final expert review to select optimal candidates from hundreds of models.

---

## Large-scale SLG (Online War Strategy Game) AI Development and Deployment (2022/10 - 2023/9)

- Led training environment optimization, feature and reward design, and high-level action development. Implemented visualization evaluation module for AI strategic decisions.
- Participated in CQL and distributed PPO algorithm development, addressing long-term feedback and data sparsity challenges.
- Led the development and deployment of online inference framework. A/B testing on new servers showed improved AI attack and defense capabilities. User satisfaction analysis indicated increased player activity and payment rates.

---

## Multi-Style Basketball Game AI Bot (2023/10 - 2025/5)

- Trained 1v1 and 3v3 offensive and defensive AI in company's proprietary basketball game. Built training environment, RL distributed training system, designed rewards, actions, and features. Used distributed PPO and Self-play framework for training and evaluation.
- Designed multiple meta-behaviors and corresponding rewards, enabling AI to execute specific styles, such as offensive tendencies for three-pointers, layups, mid-range shots, and defensive tendencies for rebounds and blocks.
- Integrated basketball domain fine-tuned ASR model and LLM to control AI style and behavior through voice or natural language input.
- Ongoing research: Following formations and tactics, learning from player data, and improving multi-agent collaboration.

---

## NBA2KX TTS Voice Synthesis System Development (2024/6 - 2024/9)

- Processed and annotated licensed commentary audio, performing precise punctuation, pause, and pronunciation adjustments (such as handling "erhua" sounds) to improve pronunciation and reduce errors.
- Built synthesis pipeline combining prompt filtering, TTS, ASR validation, and batch processing to produce high-quality voice packages. Implemented text normalization (punctuation cleaning, pronunciation correction) and weight-based long sentence segmentation strategy to ensure audio coherence and prevent truncation.

---

## ML-based NBA2KX Graphics Configuration Recommendation (2025/3 - 2025/4)

- Conducted in-depth analysis of pioneer test and S1 data, visualized performance metrics for stakeholders, proactively detected hardware-specific issues such as frame rate locking and overheating.
- Generated recommended graphics configurations for over 7,000 device models and successfully deployed machine learning model predictions during game launch.

---

## NBA2KX Intelligent QA Assistant (2025/6 - 2025/11)

- Designed MCP protocol-based multi-agent system (using Hunyuan-turbo model); implemented task planning, persona customization, and safety guardrails with average response time of 15 seconds.
- Built hybrid retrieval system (Vector/ES/MySQL) with Reranker model; designed automated pipeline and zero-downtime hot update mechanism for seamless corpus management across isolated environments.
