<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a1628,100:1a3a8f&height=120&section=header&text=Yash%20Doke&fontSize=42&fontColor=ffffff&fontAlignY=65&animation=fadeIn" width="100%"/>

### AI/ML Engineer · LLM Infrastructure · Robotics · Production ML

[![LinkedIn](https://img.shields.io/badge/LinkedIn-yash--doke-0a66c2?style=flat-square&logo=linkedin)](https://linkedin.com/in/yash-doke)
[![PyPI](https://img.shields.io/badge/PyPI-hiermem-3775a9?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/hiermem/)
[![PyPI Downloads](https://static.pepy.tech/personalized-badge/hiermem?period=total&units=INTERNATIONAL_SYSTEM&left_color=black&right_color=blue&left_text=downloads)](https://pepy.tech/projects/hiermem)
[![SkeletonGraph](https://img.shields.io/github/stars/yashdoke7/skeletongraph?style=flat-square&logo=github&label=skeletongraph&color=534AB7)](https://github.com/yashdoke7/skeletongraph)
[![HuggingFace](https://img.shields.io/badge/🤗%20Hugging%20Face-yashdoke7-ff9d00?style=flat-square)](https://huggingface.co/yashdoke7)
[![Email](https://img.shields.io/badge/Email-yashdoke215@gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:yashdoke215@gmail.com)
![Profile views](https://komarev.com/ghpvc/?username=yashdoke7&color=4a9eff&style=flat-square&label=Profile+Views)

*Rising 4th-year BE Computer Engineering @ PESMCOE, SPPU · CGPA 9.34/10*

*Building AI systems that work outside the lab — from research prototype to deployed package.*

</div>

---

## 🧠 Flagship Research — HierMem

> **LLMs forget. HierMem fixes that.**

HierMem is an OS-inspired hierarchical paged memory architecture for long-horizon LLM conversations. Inspired by virtual memory paging — the same design that lets your computer run programs larger than physical RAM — it uses a stateless curator agent, a priority-tagged constraint store, and a 4-level memory hierarchy (L0→L3) to prevent context degradation, constraint forgetting, and hallucination.

┌─────────────────────────────────────────────────────────────┐
│ Curator (~1000 tokens, constant) → reads L0 index only      │
│ Retrieval → KEYWORD / SEMANTIC / HIERARCHICAL / HYBRID      │
│ Assembler → 4-zone attention-optimised context              │
│ Main LLM → generates from bounded ~6000-token budget        │
│ Post-Proc → extracts constraints, updates L0→L3 archive     │
└─────────────────────────────────────────────────────────────┘

| Metric | Result |
|--------|--------|
| Memory compression ratio | **4.7×** vs raw context |
| Constraint survival rate | **93.3%** over long sessions |
| LLM-as-Judge score | **8.4–8.7 / 10** (vs 5.4–7.6 baselines) |
| Outperforms | RAG · RAG+Summary · MemGPT-style · Raw LLM |

[![GitHub](https://img.shields.io/badge/GitHub-llm--hiermem-181717?style=flat-square&logo=github)](https://github.com/yashdoke7/llm-hiermem)
[![PyPI](https://img.shields.io/badge/PyPI-live-3775a9?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/hiermem/)
[![PyPI Downloads](https://static.pepy.tech/personalized-badge/hiermem?period=total&units=INTERNATIONAL_SYSTEM&left_color=black&right_color=blue&left_text=downloads)](https://pepy.tech/projects/hiermem)
[![Dataset](https://img.shields.io/badge/HuggingFace-dataset-ff9d00?style=flat-square)](https://huggingface.co/yashdoke7)

---

## 🕸️ Flagship System — SkeletonGraph

> **Coding agents waste tokens re-reading code they've already seen. SkeletonGraph gives them structural memory instead.**

SkeletonGraph (SG) is the code-domain sibling of HierMem — a structure-aware retrieval layer that sits between a coding agent and its LLM. It builds a **zero-LLM** index of a repository (tree-sitter symbol graph + PageRank centrality), exposes it over the **Model Context Protocol** so any IDE agent (Claude Code, Cursor, Cline, …) can query it, and returns the *right* functions instead of whole-file dumps — so the model solves tasks in fewer turns and fewer tokens.

┌─────────────────────────────────────────────────────────────┐
│ Index → tree-sitter symbol graph + PageRank (no LLM)        │
│ Retrieve → 3-way RRF: BM25 + code-embeddings + structural   │
│ Serve → MCP tools (sg_search / sg_get / sg_expand)          │
│ Agent → Claude Code · Cursor · Cline · CLI (sg)             │
└─────────────────────────────────────────────────────────────┘

| Property | Detail |
|----------|--------|
| Index build | **Zero-LLM** — tree-sitter + PageRank, no API cost |
| Token efficiency | **≈7× fewer tokens** than Aider's repo-map at comparable solve rate (SWE-bench Verified) |
| Retrieval | 3-way RRF fusion — lexical + semantic + structural |
| Benchmarks | SWE-bench Verified & Pro · vs BM25, Aider RepoMap, graph baselines |
| Integration | Cross-IDE via MCP + portable `sg` CLI |

[![GitHub](https://img.shields.io/badge/GitHub-skeletongraph-181717?style=flat-square&logo=github)](https://github.com/yashdoke7/skeletongraph)
[![Stars](https://img.shields.io/github/stars/yashdoke7/skeletongraph?style=flat-square&color=4a9eff&logo=github)](https://github.com/yashdoke7/skeletongraph/stargazers)
![MCP](https://img.shields.io/badge/protocol-MCP-534AB7?style=flat-square)
![Index](https://img.shields.io/badge/index-zero--LLM-0f6e56?style=flat-square)

---

## 🔬 Projects

<table>
<tr>
<td width="50%" valign="top">

### [LLM Reasoning Pipeline](https://github.com/yashdoke7/llm-reasoning-pipeline)
Step-level diagnosis and targeted fine-tuning for LLM reasoning failures — finds *where* models fail, not just *if*.
- Fine-tuned Qwen 2.5 3B with QLoRA 4-bit
- **63% reduction** in step-level failure rate
- Ground-truth backtracking + error-propagation analysis
- Runs fully local via llama.cpp — zero API cost

`PyTorch` `QLoRA` `PEFT` `GGUF` `Ollama`

</td>
<td width="50%" valign="top">

### [AI-Generated Video Detection](https://github.com/yashdoke7/ai-generated-video-detection)
Deepfake detection built to stay robust across domains and shifting distributions.
- **92% AUC-ROC** across DFDC, CelebDF, WildDeepfake
- SigLIP embeddings + blockwise frame representation
- Continual learning via replay buffers + knowledge distillation
- Resists catastrophic forgetting across dataset shifts

`PyTorch` `SigLIP` `Transformers` `Continual Learning`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [Fraud Detection System](https://github.com/yashdoke7/FraudDetection)
Production-grade fraud detection — a deployed pipeline, not a demo.
- **96.2% accuracy** · **0.92 AUC-ROC**
- Processes **50K+ transactions/day**
- XGBoost + neural nets with advanced feature engineering
- Real-time FastAPI scoring with geolocation signals

`XGBoost` `FastAPI` `Neural Networks` `sklearn`
</td>
<td width="50%" valign="top">

### [Self-Evolving Multi-Agent Governance](https://github.com/Harsh-4210/Self_Evolving_Multi_Agent_Governance)
Decentralised agents that negotiate and evolve decision policies autonomously.
- PPO + quadratic voting with reputation weighting
- Agents negotiate rule proposals in a simulated economy
- PostgreSQL logging of governance events + adaptive rewards
- Delivered as a working 24-hour hackathon proof-of-concept

`Ray RLlib` `PettingZoo` `PPO` `PostgreSQL`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [AquaIntel](https://github.com/yashdoke7/AquaIntel)&nbsp;[![Stars](https://img.shields.io/github/stars/yashdoke7/AquaIntel?style=flat-square&color=4a9eff&logo=github&label=)](https://github.com/yashdoke7/AquaIntel/stargazers)
Ship-routing system with live weather integration.
- Enhanced A* with adaptive grid weighting
- Fuses wind, depth risk, and fuel efficiency in real time
- **Route update time 3.6h → 36 min** (6×)
- Full-stack with route visualisation via Leaflet.js

`TypeScript` `A* Algorithm` `OpenWeatherMap` `Leaflet.js`

</td>
<td width="50%" valign="top">

### [NutriSense](https://github.com/yashdoke7/nutrisense)
AI health platform built around generative-AI orchestration.
- Gemini 2.0 Flash for multimodal food recognition
- NLP dietary Q&A + longitudinal health-trend analysis
- Serverless GCP backend with Firestore persistence
- WCAG 2.1 accessible UI · Firebase Auth + server-side token validation

`Gemini API` `Google Cloud` `Firebase` `Vanilla CSS`

</td>
</tr>
</table>

---

## 🤖 Robotics — ABU Robocon 2026
**Team Vulcans · Software & AI Lead**
Building the autonomous navigation and AI stack for PESMCOE's entry in ABU Robocon 2026.
- Modified A\* planning for partial observability and dynamic obstacles
- PPO-based control with reward shaping for rule-compliant navigation
- ROS2 architecture + Gazebo simulation environments
- Validated in NVIDIA Isaac Sim before real-world hardware integration

`ROS2` `NVIDIA Isaac Sim` `Gazebo` `PPO` `Python` `MATLAB`

---

## ⚙️ Tech Stack

```python
LANGUAGES   = ["Python", "TypeScript", "C++", "SQL", "MATLAB"]
ML_AI       = ["PyTorch", "Hugging Face TRL", "QLoRA/PEFT", "LiteLLM",
               "LangChain", "XGBoost", "sentence-transformers", "SigLIP"]
LLM_INFRA   = ["Ollama", "llama.cpp", "GGUF", "ChromaDB", "MCP", "tree-sitter",
               "RAG pipelines", "LLM-as-Judge evaluation"]
ROBOTICS    = ["ROS2", "NVIDIA Isaac Sim", "Gazebo", "A*", "PPO", "Ray RLlib"]
BACKEND     = ["FastAPI", "Flask", "PostgreSQL", "MongoDB", "Firebase"]
CLOUD       = ["Google Cloud Platform", "AWS", "AMD Developer Cloud"]
TOOLS       = ["Git", "Docker", "pytest", "Streamlit", "Weights & Biases"]
```

---

📊 GitHub Stats

<div align="center"> <img height="180" src="https://github-readme-stats.vercel.app/api?username=yashdoke7&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=4a9eff&icon_color=4a9eff&text_color=c9d1d9&include_all_commits=true&count_private=true&cache_seconds=86400" /> <img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=yashdoke7&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=4a9eff&text_color=c9d1d9&langs_count=8&cache_seconds=86400" /> </div> <div align="center"> <img src="https://github-readme-streak-stats.herokuapp.com?user=yashdoke7&theme=github-dark-blue&hide_border=true&background=0d1117&stroke=4a9eff&ring=4a9eff&fire=ff6b35&currStreakLabel=4a9eff&dates=8b949e" /> </div> <div align="center"> <img src="https://github-profile-trophy.vercel.app/?username=yashdoke7&theme=algolia&no-frame=true&no-bg=true&column=6&margin-w=8" /> </div>

---

📈 Contribution Activity

<img src="https://github-readme-activity-graph.vercel.app/graph?username=yashdoke7&bg_color=0d1117&color=4a9eff&line=1a3a8f&point=4a9eff&area=true&area_color=1a3a8f&hide_border=true" width="100%"/>

---

🎯 Currently

🕸️ Building SkeletonGraph — structural memory for coding agents (MCP + zero-LLM index); deploying on AMD Instinct for the AMD Developer Hackathon
🔬 Extending HierMem — Needle-in-a-Haystack and multi-step reasoning benchmarks
🤖 Autonomous navigation stack for ABU Robocon 2026
📖 Rising 4th-year BE CS · Open to research internships & AI engineering roles
📬 Reach me: yashdoke215@gmail.com · linkedin.com/in/yash-doke

---

<div align="center"> <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a3a8f,100:0a1628&height=80&section=footer" width="100%"/>
"The gap between research and production is where I work."

[Show Image](https://komarev.com/ghpvc/?username=yashdoke7&color=4a9eff&style=flat-square&label=Profile+Views)

</div>
