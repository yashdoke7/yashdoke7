<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a1628,100:1a3a8f&height=150&section=header&text=Yash%20Doke&fontSize=44&fontColor=ffffff&fontAlignY=55&animation=fadeIn" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=20&duration=2800&pause=900&color=4A9EFF&center=true&vCenter=true&width=720&lines=AI%2FML+Engineer+%C2%B7+Researcher+%C2%B7+Robotics;Building+LLM+infrastructure+and+intelligent+systems;From+research+prototypes+to+deployed+systems" alt="Typing SVG" />

[![GitHub](https://img.shields.io/badge/GitHub-yashdoke7-181717?style=flat-square\&logo=github)](https://github.com/yashdoke7)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-Yash%20Doke-4285F4?style=flat-square\&logo=googlescholar\&logoColor=white)](https://scholar.google.com/citations?user=jOg2MUIAAAAJ&hl=en)
[![PyPI](https://img.shields.io/badge/PyPI-yashdoke7-3775A9?style=flat-square\&logo=pypi\&logoColor=white)](https://pypi.org/user/yashdoke7/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-yash--doke-0A66C2?style=flat-square\&logo=linkedin)](https://linkedin.com/in/yash-doke)
[![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-yashdoke7-FFD21E?style=flat-square)](https://huggingface.co/yashdoke7)
[![Email](https://img.shields.io/badge/Email-yashdoke215%40gmail.com-EA4335?style=flat-square\&logo=gmail\&logoColor=white)](mailto:yashdoke215@gmail.com)

**BE Computer Engineering @ PESMCOE, SPPU · CGPA 9.38/10**

*Building AI systems across LLM infrastructure, machine learning, and autonomous robotics.*

<br/>

<img src="https://github.com/user-attachments/assets/db1f70a4-c525-4e6f-b55e-ac8fe4e991b8" width="85%" alt="Coding animation"/>

</div>

---

## 👋 About

I build and evaluate **LLM agent systems**: retrieval and memory layers that make coding agents cheaper and assistants more private, measured with controlled experiments rather than demos. Two open-source packages on PyPI, two research preprints, and a third system, PERCH, a local-first Windows assistant.

<div align="center">

| 🏆 | 📄 | 📦 | 🤖 |
| :---: | :---: | :---: | :---: |
| **Winner**<br/>AMD Developer Hackathon Act II | **2 preprints**<br/>Research Square, 2026 | **1,400+ downloads**<br/>HierMem on PyPI | **ABU Robocon 2026**<br/>Software & AI Lead |

</div>

---

## 🧭 Featured Systems

### 🕸️ SkeletonGraph

> **Structural code retrieval for LLM coding agents. Zero-LLM index, served over MCP.**

An MCP server that gives coding agents function-level repository context, so an agent lands on the exact function to edit instead of reading whole files to find it.

<table>
<tr>
<td><b>Index</b></td>
<td>Tree-sitter symbol graph, cross-file call graph, PageRank centrality (10 languages, no LLM calls)</td>
</tr>
<tr>
<td><b>Retrieval</b></td>
<td>BM25 + code embeddings + structural rerank, fused via reciprocal rank fusion</td>
</tr>
<tr>
<td><b>Interface</b></td>
<td>MCP server + portable <code>sg</code> CLI; works with Claude Code, Codex, Cursor, Copilot, Windsurf</td>
</tr>
<tr>
<td><b>Evaluation</b></td>
<td>3,629 agent runs over 150 SWE-bench issues, Docker-verified patches, paired significance tests</td>
</tr>
</table>

**Results**

* Right file on the first search **86% of the time vs. 66%** for Claude Code's built-in search
* Matched the native agent's solve rate at **42% lower p95 (tail) cost**
* Highest recall (0.91) at the lowest token cost of any system tested, including aider's repo-map
* **Finding:** production coding agents lock their MCP tool manifest about 2 seconds after launch, silently dropping slower servers

[![PyPI](https://img.shields.io/pypi/v/skeletongraph.svg?style=flat-square&color=blue)](https://pypi.org/project/skeletongraph/)
[![Repository](https://img.shields.io/badge/GitHub-skeletongraph-181717?style=flat-square&logo=github)](https://github.com/yashdoke7/skeletongraph)
[![Stars](https://img.shields.io/github/stars/yashdoke7/skeletongraph?style=flat-square&logo=github&label=Stars)](https://github.com/yashdoke7/skeletongraph/stargazers)
[![Preprint](https://img.shields.io/badge/Preprint-Research%20Square-1a3a8f?style=flat-square)](https://doi.org/10.21203/rs.3.rs-10749266/v1)

---

### 🧠 HierMem

> **Constraint-preserving hierarchical memory for long-horizon LLM conversations.**

An OS-inspired memory layer: a four-level hierarchy (topic index, summaries, embeddings, raw turns), a small-LLM curator that retrieves only the relevant slice each turn, and a non-evictable constraint zone in every prompt.

| Evaluation (50-turn conversations, 4 domains) | Result |
| :-- | :-- |
| LLM-as-judge score | **8.46** vs. 7.15 (RAG + Summary) and 6.90 (full history) |
| Constraint survival | **93.3%** over long sessions |
| Compute cost | **36.9% lower** than full-history context |
| Memory compression | **4.7×** vs. raw context |

Won the **AMD Developer Hackathon Act II**.

[![Repository](https://img.shields.io/badge/GitHub-llm--hiermem-181717?style=flat-square&logo=github)](https://github.com/yashdoke7/llm-hiermem)
[![PyPI](https://img.shields.io/badge/PyPI-hiermem-3775A9?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/hiermem/)
[![Downloads](https://static.pepy.tech/personalized-badge/hiermem?period=total&units=INTERNATIONAL_SYSTEM&left_color=black&right_color=blue&left_text=downloads)](https://pepy.tech/projects/hiermem)
[![Preprint](https://img.shields.io/badge/Preprint-Research%20Square-1a3a8f?style=flat-square)](https://doi.org/10.21203/rs.3.rs-10055780/v1)

---

### 🪺 PERCH

> **Local-first Windows AI assistant with user-owned, privacy-typed memory.**

Summon it with a hotkey over any selection or screenshot; it answers in a panel beside your work using a local Ollama model or any OpenAI-compatible API, with an agent loop that calls tools.

<table>
<tr>
<td><b>Memory</b></td>
<td>Markdown files in six privacy-typed classes; rebuildable vector index; private requests forced local</td>
</tr>
<tr>
<td><b>Admission gate</b></td>
<td>Per-class similarity floor plus relative margin; abstains when nothing is relevant</td>
</tr>
<tr>
<td><b>Context packer</b></td>
<td>Memory and tool results share one token budget, with live eviction</td>
</tr>
<tr>
<td><b>Evaluation</b></td>
<td>Thresholds fitted by 5-fold CV on a 112-question persona, frozen, then tested on a held-out persona (69 questions)</td>
</tr>
</table>

* Held-out **F1 0.86 with zero private leaks** vs. 0.49 and 24 leaks for naive top-4 retrieval
* Benchmark is self-authored, so results are directional; paraphrased queries are the weakest case (F1 0.82)

[![Repository](https://img.shields.io/badge/GitHub-perch-181717?style=flat-square&logo=github)](https://github.com/yashdoke7/perch)
![Python](https://img.shields.io/badge/Python-Windows%2010%2F11-3776AB?style=flat-square&logo=python&logoColor=white)

---

## 📄 Publications

* **SkeletonGraph: A Zero-LLM Structural Retrieval Engine for Coding Agents, and Why Its Gains Land in the Cost Tail, Not the Median.** Research Square preprint, 2026. [doi:10.21203/rs.3.rs-10749266/v1](https://doi.org/10.21203/rs.3.rs-10749266/v1)
* **HierMem: Hierarchical Memory for Long-Horizon LLM Conversations.** Research Square preprint, 2026. [doi:10.21203/rs.3.rs-10055780/v1](https://doi.org/10.21203/rs.3.rs-10055780/v1)

---

## 🔬 More Projects

<table>
<tr>
<td width="50%" valign="top">

### [LLM Reasoning Pipeline](https://github.com/yashdoke7/llm-reasoning-pipeline)

Step-level diagnosis and targeted fine-tuning of small-LLM reasoning.

* QLoRA fine-tune of Qwen2.5-3B: accuracy **62.5% → 76.3%**
* Ground-truth backtracking and error-propagation analysis
* GGUF export for local inference

`PyTorch` `QLoRA` `PEFT` `GGUF`

</td>
<td width="50%" valign="top">

### [AI-Generated Video Detection](https://github.com/yashdoke7/ai-generated-video-detection)

Deepfake detection built for robustness under dataset shift.

* **92% AUC-ROC** across benchmark datasets
* SigLIP representations, replay buffers, knowledge distillation
* Continual-learning pipeline against catastrophic forgetting

`PyTorch` `SigLIP` `Transformers` `Continual Learning`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [Fraud Detection System](https://github.com/yashdoke7/FraudDetection)

End-to-end ML pipeline for real-time fraud scoring.

* **96.2% accuracy**, **0.92 AUC-ROC**
* XGBoost and neural networks on transactional and geolocation features
* FastAPI inference service

`XGBoost` `FastAPI` `scikit-learn`

</td>
<td width="50%" valign="top">

### [Self-Evolving Multi-Agent Governance](https://github.com/Harsh-4210/Self_Evolving_Multi_Agent_Governance)

Multi-agent governance simulation with adaptive policies (collaboration).

* PPO agents with quadratic voting
* Reputation-weighted decisions and adaptive rewards

`Ray RLlib` `PettingZoo` `PPO` `PostgreSQL`

</td>
</tr>
</table>

Also: [AquaIntel](https://github.com/yashdoke7/AquaIntel) (weather-aware ship routing with enhanced A\*; data pipeline cut from 3.6 h to 36 min) · [NutriSense](https://github.com/yashdoke7/nutrisense) (Gemini-based multimodal food and nutrition analysis)

---

## 🤖 Robotics

**ABU Robocon 2026 · Team Vulcans · Software & AI Lead.** Autonomous navigation and perception for PESMCOE's robots: path planning under partial observability, real-time computer vision, ROS2 architecture, and simulation in NVIDIA Isaac Sim and Gazebo, integrated with embedded controllers.

`ROS2` `Isaac Sim` `Gazebo` `Python` `C++` `Computer Vision`

---

## ⚙️ Technical Stack

<table>
<tr><td><b>Languages</b></td><td>Python · C++ · TypeScript · SQL</td></tr>
<tr><td><b>ML & LLMs</b></td><td>PyTorch · Transformers · QLoRA/PEFT · RAG · MCP · Ollama · llama.cpp · LiteLLM · tree-sitter</td></tr>
<tr><td><b>Robotics</b></td><td>ROS2 · NVIDIA Isaac Sim · Gazebo · Reinforcement Learning</td></tr>
<tr><td><b>Backend & Tools</b></td><td>FastAPI · PostgreSQL · Firebase · Docker · Git · pytest · Google Cloud · AWS</td></tr>
</table>

---

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=yashdoke7&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=4a9eff&icon_color=4a9eff&text_color=c9d1d9&include_all_commits=true&count_private=true" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=yashdoke7&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=4a9eff&text_color=c9d1d9&langs_count=6" />

<br/><br/>

*"The gap between research and production is where I work."*

</div>
