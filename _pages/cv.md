---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **M.S. in Computer Science and Technology**, Beijing Jiaotong University, 2019.9 - 2022.4
* **B.S. in Digital Media Technology**, Harbin Institute of Technology, 2015.9 - 2019.5

Work Experience
======
* **Game AI Engineer (Applied Research)**, Tencent IEG — Shanghai, 2023.10 - Present
  * Multi-style basketball game AI bot development
  * NBA2KX TTS voice synthesis system development
  * ML-based graphics configuration recommendation
  * Intelligent QA assistant based on MCP protocol

* **Reinforcement Learning Algorithm Engineer**, NetEase Games AI Lab — Shanghai, 2022.5 - 2023.9
  * Large-scale SLG AI development and deployment

* **Reinforcement Learning Algorithm Intern**, NetEase Games AI Lab — Shanghai, 2021.6 - 2021.9

Awards
======
* **2023** - IJCAI AI Olympics Competition (1st/40, Oral Presentation)
* **2023** - CoG Google Research Football Multi-Agent AI Competition (2nd/20)
* **2022** - CoG Google Research Football Multi-Agent AI Competition (1st/20)
* **2021** - CoG FightingICE Fighting Game AI Competition (1st/15)
* **2020** - SMARTS DAI Autonomous Driving Single-Agent Track (7th/70)
* **2020** - KDD CUP Reinforcement Learning Track: Ride-Hailing Order Dispatch (6th/150)

Skills
======
* **RL Algorithms**: Large-scale Distributed RL, Self-Play, Model-based RL, Multi-agent RL, Offline RL, RLHF, RLVR
* **LLMs**: Transformer, etc.
* **Programming**: C, Python, PyTorch, TensorFlow
* **Other Technologies**: Git, Linux, VSCode

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Projects
======
* **IEEE CoG2021 Fighting Game AI Competition** (2021.6 - 2021.8)
  * Won the championship with 100% win rate in PVE speedrun and PVP three-character tracks
  * Developed distributed Population-Based Training (PBT) framework for fighting games

* **IEEE CoG2022 Google Research Football Multi-Agent AI Competition** (2022.5 - 2022.9)
  * Analyzed top single-agent football solutions, built features and rewards
  * Implemented large-scale distributed PPO training with innovative hybrid opponent pool sampling

* **Large-scale SLG AI Development & Deployment** (2022.10 - 2023.9)
  * Led training environment optimization, feature and reward design
  * Participated in CQL and distributed PPO algorithm development

* **Multi-style Basketball Game AI Bot** (2023.10 - 2025.5)
  * Trained 1v1 and 3v3 offensive/defensive AI using distributed PPO and Self-play
  * Integrated ASR and LLM for voice/natural language AI control

* **NBA2KX TTS Voice Synthesis System** (2024.6 - 2024.9)
  * Built synthesis pipeline with prompt filtering, TTS, ASR verification

* **ML-based NBA2KX Graphics Configuration Recommendation** (2025.3 - 2025.4)
  * Generated recommended configurations for 7000+ device models

* **NBA2KX Intelligent QA Assistant** (2025.6 - 2025.11)
  * Designed multi-agent system based on MCP protocol with 15s average response time
  * Built hybrid retrieval system (Vector/ES/MySQL) with Reranker model
