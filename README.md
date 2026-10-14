# MedLitSearchSkill 🔬🤖

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Tested On](https://img.shields.io/badge/Models-Doubao%20%7C%20Qwen-00E5FF.svg)](#supported-models)
[![YouTube Video](https://img.shields.io/badge/YouTube-Watch%20Demo-red.svg)](https://www.youtube.com/@TheReproGuy)

A structured, anti-hallucination **Skill module** designed to empower AI Agents (specifically **Doubao** and **Qwen**) to retrieve, verify, and summarize medical literature with real PMIDs, DOIs, and validated clinical metrics.

---

## 🎯 The Problem

When using general-purpose LLMs for medical paper retrieval, researchers often encounter severe **scientific hallucinations**:
- ❌ Fake papers, invalid DOIs, or fabricated PMIDs
- ❌ Mismatched abstracts and hallucinated statistical figures (e.g., HR, AUC, sample sizes)
- ❌ Dead or broken external links

## 💡 What This Skill Does

By imposing strict verification pipelines and structured retrieval rules, this Skill forces the agent to:
1. **Anchor Citations**: Verify all references against trusted indexing databases (PubMed / Crossref).
2. **Eliminate Fake Links**: Ensure every returned article contains a real, navigable direct link.
3. **Strict Data Extraction**: Extract exact metrics without paraphrasing numbers or hallucinating outcomes.
4. **Structured Categorization**: Group results by evidence level (e.g., RCTs, Real-World Studies, Medical Imaging).

---

## 📦 Files in This Repository

| File | Supported Agent | Format | Description |
| :--- | :--- | :--- | :--- |
| `doubao_med_lit_search.md` | **Doubao (豆包)** | Markdown (`.md`) | Direct drag-and-drop into Doubao Work Skills |
| `qwen_med_lit_search.zip` | **Qwen (千问)** | ZIP Archive (`.zip`) | Packaged skill compliant with Qwen Workspace format |

---

## 🚀 Quick Setup

### 1. Doubao (豆包)
1. Navigate to **Work (工作)** mode in Doubao.
2. Go to **Skill Management (技能管理)** $\rightarrow$ **Upload Skill (上传技能)**.
3. Drag and drop the `.md` file.
4. Activate the skill and run your literature search query.

### 2. Qwen (千问)
1. Switch to **Work (工作)** mode in Qwen.
2. Go to **Skills (技能)** $\rightarrow$ **Manage Skills (管理技能)** $\rightarrow$ **Upload Skill (上传技能)**.
3. Upload the `.zip` archive.
4. Once verified, enable the skill and start researching.

---

## 🧪 Benchmark & Verification

In our dual-model benchmark (HCC-TACE immunotherapy medical imaging study), upgrading vanilla models with this Skill yielded:
- **100% Real Literature Links**: All PMIDs directly navigable.
- **Zero Fabricated Metrics**: Accurate alignment with published abstracts (HR, AUC, sample sizes).
- Performance comparable to GPT-level research assistants.

📺 **Full benchmark & walkthrough video:**  
[Watch on YouTube](https://www.youtube.com/@TheReproGuy)

---

## 👤 About TheReproGuy

I reproduce medical AI research papers and evaluate whether published computational methods and AI agents work reliably in real-world clinical research.

- **Topics**: Medical Imaging AI | Radiomics | LLM Agents for Science | PyRadiomics / MONAI Workflows
- **Philosophy**: Paper $\rightarrow$ Code $\rightarrow$ Experiments $\rightarrow$ Verification

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
