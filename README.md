# Hi, I'm Yanjie Liang (梁延杰) 👋

<p>
  <a href="https://github.com/momomoxiaobai"><img src="https://img.shields.io/badge/GitHub-momomoxiaobai-181717?style=flat&logo=github" alt="GitHub"></a>
  <a href="mailto:mxiaobai10@163.com"><img src="https://img.shields.io/badge/Email-mxiaobai10@163.com-EA4335?style=flat&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://github.com/AIGeeksGroup/PresentAgent"><img src="https://img.shields.io/github/stars/AIGeeksGroup/PresentAgent?style=flat&logo=github&label=PresentAgent" alt="PresentAgent stars"></a>
</p>

LLM Algorithm Engineer at **ByteDance**. I work on large language models and multimodal agents.

```python
interests = [
    "LLM",
    "RL Post-Training",
    "Pre-training Model Evals / Benchmark Construction",
    "Agent Benchmark",
    "LLM-based Agents",
    "Multimodal LLM & Document Intelligence",
]
```

---

## 📄 Publications

> `*` denotes equal contribution. **Bold** denotes my name.

### 🥇 First / Co-first Author

- **PresentAgent: Multimodal Agent for Presentation Video Generation** <br>
  Jingwei Shi\*, Zeyu Zhang\*, Biao Wu\*, **Yanjie Liang**\*, Meng Fang, Ling Chen, Yang Zhao <br>
  *EMNLP 2025 (System Demonstrations), CCF-B*
  · [[Paper]](https://aclanthology.org/2025.emnlp-demos.58/)
  · [[arXiv]](https://arxiv.org/abs/2507.04036)
  · [[Code ⭐140+]](https://github.com/AIGeeksGroup/PresentAgent)
  · [[Dataset]](https://huggingface.co/datasets/AIGeeksGroup/Doc2Present)

- **MTAD: A Three-Stage Framework for Machine Translation Agents Distillation** <br>
  Xuanbo Guo\*, **Yanjie Liang**\*, Jianxiang Zhou, Baqun Sun, Ke Wang <br>
  *ICASSP 2026, CCF-B*
  · [[IEEE]](https://ieeexplore.ieee.org/document/11462599)

### 🥈 Co-author

- **Infinity-Parser: Layout-Aware Reinforcement Learning for Scanned Document Parsing** <br>
  Baode Wang, Biao Wu, Weizhen Li, Meng Fang, Zuming Huang, Jun Huang, **Yanjie Liang**, Haozhe Wang, Ling Chen, Wei Chu, Yuan Qi <br>
  *Findings of ACL 2026, CCF-A*
  · [[Paper]](https://aclanthology.org/2026.findings-acl.82/)
  · [[PDF]](https://aclanthology.org/2026.findings-acl.82.pdf)

- **Inducing Argument Facets for Faithful Opinion Summarization** <br>
  Jian Wang, **Yanjie Liang**, Yuqing Sun, Bin Gong <br>
  *Findings of EMNLP 2025, CCF-B*
  · [[Paper]](https://aclanthology.org/2025.findings-emnlp.876/)

- **ALSA: Context-Sensitive Prompt Privacy Preservation in Large Language Models** <br>
  Hongru Ma, Wenpeng Lu, **Yanjie Liang**, Tianyi Wang, Qi Zhang, Yingjie Zhu, Jiasheng Si <br>
  *KDD 2025, CCF-A*
  · [[Paper]](https://dl.acm.org/doi/10.1145/3711896.3736840)

- **Iteratively Calibrating Prompts for Unsupervised Diverse Opinion Summarization** <br>
  Jian Wang, **Yanjie Liang**, Yuqing Sun, Xin Li <br>
  *ECAI 2024, CCF-B*

- **EvioSum: An Evidence-Guided Generation Framework for Faithful and Interpretable Opinion Summarization** <br>
  Jian Wang, **Yanjie Liang**, Yuqing Sun, Xin Li <br>
  *Findings of ACL 2026, CCF-A*
  · [[ACM]](https://dl.acm.org/doi/10.1145/3773966.3777962)

<!-- TODO: 下面两篇实习期间的在投论文，补齐作者与链接后把注释去掉
### 📝 Under Review

- **MMM: A Multi-Agent System with Novel LQA Paradigm for Multilingual Machine Translation** <br>
  `AUTHOR LIST TBD` <br>
  *Under review at WWW, CCF-A* · *ByteDance internship*
- **Autonomous Project-Level Code Generation without External Knowledge** <br>
  `AUTHOR LIST TBD` <br>
  *Under review at CIKM, CCF-B*
-->

---

## 📰 News

- **[2026.07]** 🎉 Two papers accepted: **Infinity-Parser** and **EvioSum** to *Findings of ACL 2026*.
- **[2025.11]** 🎉 **PresentAgent** and **Inducing Argument Facets** accepted to *EMNLP 2025* (Demo + Findings).
- **[2025.08]** 🎉 **ALSA** accepted to *KDD 2025*.
- **[2025.06]** 🚀 **PresentAgent** code and the **Doc2Present** dataset are open-sourced.

---

## 🔬 Research

<details open>
<summary><b>PresentAgent</b> — Document-to-Presentation-Video Generation</summary>

We introduce the new task of automatically generating a structured slide video with narration from long
documents. **PresentAgent** is a modular framework that covers document parsing, layout-aware slide
construction, script writing and audio-visual synchronization, enabling controllable and interpretable
video generation. We further propose **PresentEval**, a VLM-driven multi-dimensional evaluation protocol
that scores generated videos along content, visual and comprehension axes, together with an open-source
high-quality benchmark.

</details>

<details>
<summary><b>Infinity-Parser</b> — Layout-Aware RL for Scanned Document Parsing</summary>

**layoutRL** is an end-to-end reinforcement learning framework that optimizes a composite reward over
normalized edit distance, paragraph-count accuracy and reading-order preservation, so the model learns to
explicitly perceive layout. Built on **Infinity-Doc-55K** and plugged into the vision-language parser
Infinity-Parser, it reaches SoTA accuracy and structural fidelity on Chinese/English OCR, table and formula
extraction and reading-order detection — surpassing GPT-4o and Qwen2.5-VL-72B.

</details>

<details>
<summary><b>Translation Agents</b> — MMM / MTAD</summary>

We systematize the LQA (translation quality assessment) paradigm and build the **AILQA Agent**, which
leverages LLMs for efficient and accurate evaluation while greatly reducing human annotation cost. On top
of it, **MMMTrans Agent** forms a closed loop of *initial translation → autonomous LQA → quality refinement*.
**MTAD** takes this further with a three-stage distillation framework: distill AILQA → distill TransAgent →
use the distilled LQA model as the reward model for GRPO.

</details>

<details>
<summary><b>Privacy-Preserving & Faithful Generation</b> — ALSA / opinion summarization</summary>

**ALSA** is a context-sensitive prompt privacy preservation framework: a three-dimensional scoring mechanism
(PLRS / CIIS / TRS) dynamically quantifies how replaceable and how private each token in a prompt is, and
clustering then determines the anonymization action (keep / replace / encrypt / delete) per span, balancing
privacy, semantics and task relevance. On the summarization side, I work on RL-based prompt calibration
(ECAI 2024), argument-facet-guided faithful summarization (EMNLP Findings 2025) and evidence-guided
interpretable summarization (EvioSum, ACL Findings 2026).

</details>

---

## 🚀 Open Source

- **[AIGeeksGroup/PresentAgent](https://github.com/AIGeeksGroup/PresentAgent)** ⭐ 140+ — official code and demo for our EMNLP 2025 demo paper, with the **Doc2Present** dataset released on [Hugging Face](https://huggingface.co/datasets/AIGeeksGroup/Doc2Present).
- **[infly-ai/INF-MLLM](https://github.com/infly-ai/INF-MLLM)** ⭐ 250+ — open-source multimodal LLMs for SOTA visual-language understanding and advanced document intelligence; developed during my internship at Infinigence AI (无限光年), where the layout-aware parsing work above was born.

---

## 🛠 Skills

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat&logo=nvidia&logoColor=white)
![DeepSpeed](https://img.shields.io/badge/DeepSpeed-0078D4?style=flat&logo=microsoft&logoColor=white)
![Megatron](https://img.shields.io/badge/Megatron--LM-1F425F?style=flat&logo=nvidia&logoColor=white)
![vLLM](https://img.shields.io/badge/vLLM-FF6F00?style=flat)
![SGLang](https://img.shields.io/badge/SGLang-4B8BBE?style=flat)
![Ray](https://img.shields.io/badge/Ray-028CF0?style=flat&logo=ray&logoColor=white)
![Triton](https://img.shields.io/badge/Triton-6E4AFF?style=flat)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat&logo=latex&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

**LLM** — pre-training & SFT data pipelines, RL post-training (PPO / GRPO / DPO), reward modeling, long-context training. <br>
**Evals** — benchmark construction for pre-trained models and agents, LLM-as-a-Judge, human & automatic evaluation protocols. <br>
**Agents** — multi-agent orchestration, tool use, multimodal document & video generation pipelines.

---

## 📫 Contact

- **Email:** mxiaobai10@163.com
- **GitHub:** [@momomoxiaobai](https://github.com/momomoxiaobai)
- **Website / Blog:** [momomoxiaobai.github.io](https://momomoxiaobai.github.io)

<p align="center"><i>Always happy to talk about LLMs, RL post-training, and benchmarks.</i></p>
