<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a1628,100:1a3a8f&height=150&section=header&text=Yash%20Doke&fontSize=44&fontColor=ffffff&fontAlignY=55&animation=fadeIn" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=20&duration=2800&pause=900&color=4A9EFF&center=true&vCenter=true&width=720&lines=AI%2FML+Engineer+%C2%B7+Researcher+%C2%B7+Robotics;Building+LLM+infrastructure+and+intelligent+systems;From+research+prototypes+to+deployed+systems" alt="Typing SVG" />

[![GitHub](https://img.shields.io/badge/GitHub-yashdoke7-181717?style=flat-square\&logo=github)](https://github.com/yashdoke7)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-Yash%20Doke-4285F4?style=flat-square\&logo=googlescholar\&logoColor=white)](https://scholar.google.com/citations?user=jOg2MUIAAAAJ&hl=en)
[![PyPI](https://img.shields.io/badge/PyPI-yashdoke7-3775A9?style=flat-square\&logo=pypi\&logoColor=white)](https://pypi.org/user/yashdoke7/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-yash--doke-0A66C2?style=flat-square\&logo=linkedin)](https://linkedin.com/in/yash-doke)
[![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-yashdoke7-FFD21E?style=flat-square)](https://huggingface.co/yashdoke7)
[![Email](https://img.shields.io/badge/Email-yashdoke215%40gmail.com-EA4335?style=flat-square\&logo=gmail\&logoColor=white)](mailto:yashdoke215@gmail.com)

**BE Computer Engineering @ PESMCOE, SPPU · CGPA 9.34/10**

*Building AI systems across LLM infrastructure, machine learning, and autonomous robotics.*

<br/>

<img src="https://github.com/user-attachments/assets/db1f70a4-c525-4e6f-b55e-ac8fe4e991b8" width="85%" alt="Coding animation"/>

</div>

---

## 🕸️ SkeletonGraph

> **Structural code retrieval for LLM coding agents.**

SkeletonGraph is a structure-aware retrieval layer for coding agents. It builds a **zero-LLM repository index** from source code structure and exposes targeted retrieval through the **Model Context Protocol (MCP)**, helping agents retrieve relevant symbols and dependencies instead of repeatedly consuming entire files.

<table>
<tr>
<td><b>Index</b></td>
<td>tree-sitter symbol graph + PageRank centrality</td>
</tr>
<tr>
<td><b>Retrieval</b></td>
<td>BM25 + code embeddings + structural signals via RRF</td>
</tr>
<tr>
<td><b>Interface</b></td>
<td>MCP tools + portable <code>sg</code> CLI</td>
</tr>
<tr>
<td><b>Evaluation</b></td>
<td>SWE-bench Verified & Pro</td>
</tr>
</table>

**Highlights**

* **Zero-LLM indexing** — repository structure is built without API calls
* Hybrid lexical, semantic, and structural retrieval
* Cross-file dependency graph built through tree-sitter parsing
* MCP integration for use with compatible coding agents and IDE workflows
* Benchmarked against BM25, repository-map, and graph-based retrieval baselines

[![Repository](https://img.shields.io/badge/GitHub-skeletongraph-181717?style=flat-square\&logo=github)](https://github.com/yashdoke7/skeletongraph)
[![Stars](https://img.shields.io/github/stars/yashdoke7/skeletongraph?style=flat-square\&logo=github\&label=Stars)](https://github.com/yashdoke7/skeletongraph/stargazers)
![MCP](https://img.shields.io/badge/Protocol-MCP-534AB7?style=flat-square)
![Index](https://img.shields.io/badge/Index-Zero--LLM-0F6E56?style=flat-square)

---

## 🧠 HierMem

> **Constraint-preserving hierarchical memory for long-horizon LLM conversations.**

HierMem is an OS-inspired hierarchical memory architecture designed to preserve constraints and relevant context across long conversations. Inspired by virtual-memory paging, it combines a lightweight curator, a priority-aware constraint store, and a multi-level memory hierarchy to manage context under a bounded token budget.

<table>
<tr>
<td><b>Curator</b></td>
<td>Reads a compact L0 index to identify relevant memory</td>
</tr>
<tr>
<td><b>Retrieval</b></td>
<td>Keyword · Semantic · Hierarchical · Hybrid</td>
</tr>
<tr>
<td><b>Assembly</b></td>
<td>Attention-aware bounded context construction</td>
</tr>
<tr>
<td><b>Memory</b></td>
<td>Constraint extraction and hierarchical L0 → L3 archival</td>
</tr>
</table>

| Evaluation          | Result                                           |
| :------------------ | :----------------------------------------------- |
| Memory compression  | **4.7×** vs. raw context                         |
| Constraint survival | **93.3%** over long sessions                     |
| LLM-as-Judge        | **8.4–8.7 / 10**                                 |
| Evaluated against   | RAG · RAG + Summary · MemGPT-style · Raw context |

[![Repository](https://img.shields.io/badge/GitHub-llm--hiermem-181717?style=flat-square\&logo=github)](https://github.com/yashdoke7/llm-hiermem)
[![PyPI](https://img.shields.io/badge/PyPI-hiermem-3775A9?style=flat-square\&logo=pypi\&logoColor=white)](https://pypi.org/project/hiermem/)
[![Downloads](https://static.pepy.tech/personalized-badge/hiermem?period=total\&units=INTERNATIONAL_SYSTEM\&left_color=black\&right_color=blue\&left_text=downloads)](https://pepy.tech/projects/hiermem)

---

## 🔬 Selected Projects

<table>
<tr>
<td width="50%" valign="top">

### [LLM Reasoning Pipeline](https://github.com/yashdoke7/llm-reasoning-pipeline)

Step-level diagnosis and targeted fine-tuning for LLM reasoning failures.

* QLoRA 4-bit fine-tuning of Qwen 2.5 3B
* **63% reduction** in step-level failure rate
* Ground-truth backtracking and error-propagation analysis
* Local inference through llama.cpp

<br/>

`PyTorch` `QLoRA` `PEFT` `GGUF`

</td>
<td width="50%" valign="top">

### [AI-Generated Video Detection](https://github.com/yashdoke7/ai-generated-video-detection)

Deepfake detection designed for robustness across changing data distributions.

* **92% AUC-ROC** across multiple benchmark datasets
* SigLIP-based visual representations
* Replay buffers and knowledge distillation
* Continual-learning pipeline for dataset shifts

<br/>

`PyTorch` `SigLIP` `Transformers` `Continual Learning`

</td>
</tr>

<tr>
<td width="50%" valign="top">

### [AquaIntel](https://github.com/yashdoke7/AquaIntel)

Weather-aware ship-route optimisation using adaptive path planning.

* Enhanced A* with dynamic grid weighting
* Live weather and environmental signals
* Data-update pipeline reduced from **3.6 h to 36 min**
* Interactive route visualisation

<br/>

`Python` `A*` `OpenWeatherMap` `Leaflet.js`

</td>
<td width="50%" valign="top">

### [Fraud Detection System](https://github.com/yashdoke7/FraudDetection)

End-to-end machine-learning pipeline for real-time fraud scoring.

* **96.2% accuracy** and **0.92 AUC-ROC**
* XGBoost and neural-network models
* Feature engineering with transactional and geolocation signals
* FastAPI-based inference service

<br/>

`XGBoost` `FastAPI` `scikit-learn` `Neural Networks`

</td>
</tr>

<tr>
<td width="50%" valign="top">

### [NutriSense](https://github.com/yashdoke7/nutrisense)

Multimodal AI platform for food analysis and nutrition-oriented insights.

* Gemini-based multimodal food recognition
* Dietary Q&A and longitudinal trend analysis
* Cloud-hosted backend with persistent user data
* Authentication and accessible web interface

<br/>

`Gemini API` `Google Cloud` `Firebase` `FastAPI`

</td>
<td width="50%" valign="top">

### [Self-Evolving Multi-Agent Governance](https://github.com/Harsh-4210/Self_Evolving_Multi_Agent_Governance)

Multi-agent governance simulation with adaptive decision policies.

* PPO-based agents and quadratic voting
* Reputation-weighted decision mechanisms
* Adaptive reward structures
* Governance-event logging and analysis

<br/>

`Ray RLlib` `PettingZoo` `PPO` `PostgreSQL`

</td>
</tr>
</table>

---

## 🤖 Robotics

### ABU Robocon 2026 · Team Vulcans

**Software & AI Lead**

Developing autonomous navigation and perception systems for PESMCOE's ABU Robocon 2026 robots.

* Path planning under partial observability and dynamic obstacles
* Computer vision and real-time perception pipelines
* ROS2-based software architecture
* Simulation and validation using NVIDIA Isaac Sim and Gazebo
* Integration with embedded controllers and physical robot hardware

`ROS2` `NVIDIA Isaac Sim` `Gazebo` `Python` `C++` `Computer Vision`

---

## ⚙️ Technical Stack

<table>
<tr>
<td><b>Languages</b></td>
<td>Python · C++ · TypeScript · SQL · MATLAB</td>
</tr>
<tr>
<td><b>Machine Learning</b></td>
<td>PyTorch · Transformers · QLoRA/PEFT · XGBoost · SigLIP · sentence-transformers</td>
</tr>
<tr>
<td><b>LLM Systems</b></td>
<td>Ollama · llama.cpp · GGUF · LiteLLM · RAG · MCP · tree-sitter</td>
</tr>
<tr>
<td><b>Robotics</b></td>
<td>ROS2 · NVIDIA Isaac Sim · Gazebo · Path Planning · Reinforcement Learning</td>
</tr>
<tr>
<td><b>Backend & Data</b></td>
<td>FastAPI · Flask · PostgreSQL · MongoDB · Firebase</td>
</tr>
<tr>
<td><b>Cloud & Tools</b></td>
<td>Google Cloud · AWS · AMD Developer Cloud · Docker · Git · pytest</td>
</tr>
</table>

---

## 📊 GitHub Activity

<div align="center">

<img height="175" src="https://github-readme-stats.vercel.app/api?username=yashdoke7&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=4a9eff&icon_color=4a9eff&text_color=c9d1d9&include_all_commits=true&count_private=true" />

<img height="175" src="https://github-readme-stats.vercel.app/api/top-langs/?username=yashdoke7&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=4a9eff&text_color=c9d1d9&langs_count=8" />

</div>

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=yashdoke7&bg_color=0d1117&color=4a9eff&line=1a3a8f&point=4a9eff&area=true&area_color=1a3a8f&hide_border=true" width="100%"/>

---

<div align="center">

[![Profile Views](https://komarev.com/ghpvc/?username=yashdoke7\&color=4a9eff\&style=flat-square\&label=Profile+Views)](https://github.com/yashdoke7)

<br/><br/>

*"The gap between research and production is where I work."*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a3a8f,100:0a1628&height=90&section=footer" width="100%"/>

</div>
