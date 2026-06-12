# Getting Started with AI Coding and Notebooks

**Date:** June 17, 2026

A hands-on session exploring the landscape of AI-enabled data analysis workflows. If you can upload a CSV to ChatGPT and get results, why use a notebook? This webinar answers that question by showing when—and when not—to use notebooks for AI-powered analysis.

## The Core Question

**"If I can upload my data to ChatGPT or Claude, why would I write a notebook?"**

It's a fair question. And the answer isn't "notebooks are always better." This webinar shows you the landscape, when to use each approach, and why notebooks become valuable as your analysis scales.

## What You'll Learn

By the end of this session, you'll understand:

1. **Level 1** - When to use AI chat interfaces directly (fast, no coding needed, but limited for scale)
2. **Level 2** – Why notebooks matter when you need to repeat analysis across many records consistently
3. **Level 3** – How to combine notebooks with AI APIs to automate analysis at scale
4. **Level 4** – That open-source models exist and when they might be useful

**The key insight:** You'll move from "AI answers one question at a time" to "AI systematically processes hundreds of records with reproducible logic."

---

## Four Ways to Analyze Data with AI

We'll explore the same research question using four different approaches. Each has trade-offs in terms of ease, scalability, and repeatability.

| Approach | Easy | Scalable | Repeatable | Best For |
|----------|------|----------|-----------|----------|
| **Chat Interface** (ChatGPT/Claude) | ✓ | ✗ | ✗ | Quick exploration, one-time questions |
| **Notebook (No AI)** | Medium | Medium | ✓ | Structured analysis, before you need AI |
| **Notebook + API** | ✓ | ✓ | ✓ | **The sweet spot** – automate analysis at scale |
| **Notebook + Local Model** | Medium | ✓ | ✓ | Control, privacy, offline work |

---

## The Notebooks: Same Question, Different Approaches

### 1. **Notebook Without AI** (`Notebook_without_AI.ipynb`)

**What it does:** Analyzes the data using traditional Python (pandas, basic statistics, charts).

**Why start here?** 
- Establishes a baseline.
- Shows that notebooks existed before generative AI
- Demonstrates reproducible, transparent analysis

**Key learning:** Notebooks aren't just for "doing AI"—they're for creating well-documented, repeatable workflows.

---

### 2. **Notebook with API** (`Notebook_with_API.ipynb`)

**What it does:** Same question, same dataset. But now AI processes every record systematically.

```python
for record in dataset:
    result = ai_api.analyze(record)  # Repeated, consistent analysis
```

**Why this matters:**
- Moves from single-shot analysis to **batch processing**
- Every time you run it, you get the same results (reproducibility)
- You can scale to 100s or 1000s of records, not just one

**Use cases:**
- Categorize responses automatically
- Summarize themes from feedback
- Extract structured data from unstructured text
- Generate insights across your entire dataset

**Key learning:** This is where the notebook becomes powerful. AI becomes a processing engine, not just an answer engine.

---

### 3. **Notebook with HuggingFace Model** (`Notebook_with_HFmodel.ipynb`)

**What it does:** Same analysis, but using a local AI model instead of an API.

**Why consider this?**
- **Control:** You choose the model, version, and parameters
- **Privacy:** Data never leaves your machine or server
- **No API costs:** One-time download, then it's free
- **Offline:** Works without internet connectivity

**Trade-offs:**
- More technical setup required
- Need sufficient compute resources
- Model quality varies by task

**Key learning:** AI doesn't always mean "ChatGPT" or external APIs. Open-source models give you options and control.

---

## How to Use This Repo

**Launch notebooks instantly in Google Colab (no setup required):**

| Notebook | Launch in Colab |
|----------|-----------------|
| Notebook Without AI | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ms-cc-org/Webinar3-Getting-Started-with-AI-Coding-and-Notebooks/blob/main/Notebook_without_AI.ipynb) |
| Notebook with API | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ms-cc-org/Webinar3-Getting-Started-with-AI-Coding-and-Notebooks/blob/main/Notebook_with_API.ipynb) |
| Notebook with HuggingFace Model | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ms-cc-org/Webinar3-Getting-Started-with-AI-Coding-and-Notebooks/blob/main/Notebook_with_HFmodel.ipynb) |

**During the Webinar:**

1. **Click a notebook link above** – It opens instantly in Google Colab (no installation needed)
2. **Start with the chat interface question:** We'll begin by solving a problem using ChatGPT or Claude directly (the approach you probably already use).
3. **Open Notebook Without AI:** See the same problem solved with traditional Python—showing what's possible without AI.
4. **Run Notebook with API:** Discover how to automate analysis and scale to multiple records. This is typically the "aha moment."
5. **Explore Notebook with Local Model:** See that open-source models are accessible and sometimes better for your use case.
6. **Compare the results:** Notice that all three notebooks produce similar, reproducible outputs—the real value is in the automation and consistency.

---

## The Real Value of Notebooks

After ChatGPT, the question isn't "how do I use AI?" It's "how do I use AI **reproducibly**?"

Imagine six months from now, someone asks: *"Can you rerun that analysis on the new data?"*

**With ChatGPT:**
- Find the old conversation
- Remember what you asked
- Hope the results are similar

**With a notebook:**
```python
load_data()
analyze()
visualize()
report()
```
Run it. Done. Same results, every time.

That's the notebook advantage: **it's a well-documented, reproducible workflow.**

---

## What You Should Leave Understanding

- **Level 1:** I can use ChatGPT directly on data for quick exploration  
- **Level 2:** I understand when a notebook becomes useful (scale, repeatability)  
- **Level 3:** I can combine notebooks and AI APIs to automate analysis  
- **Level 4:** I know open-source models exist and when they might matter  

If you leave with these four mental models, you've successfully bridged the gap between "AI user" and "AI practitioner."

---

## What's Next?

After this webinar, you're ready for:

- **Build your own notebooks** for your research, teaching, or analysis
- **Explore the AI Accelerator** – deeper technical training on model fine-tuning, deployment, and advanced workflows
- **Participate in hackathons** – apply these skills on real-world projects
- **Engage technical consulting** – bring in experts for domain-specific applications