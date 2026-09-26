<h1 align="center">Hey, I'm An 👋</h1>

<p align="center">
  <em>Applied AI Engineer • Computer Science @ UIT – VNU-HCM</em>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/an-nguyen-tran-khuong/">LinkedIn</a> •
  <a href="https://scholar.google.com/citations?user=DSbVqkIAAAAJ&hl=en">Google Scholar</a> •
  <a href="mailto:ankhuong.working@gmail.com">Email</a>
</p>

<p align="center">
  <img alt="AI" src="https://img.shields.io/badge/AI-Engineering-6C63FF?style=flat-square" />
  <img alt="Machine Learning" src="https://img.shields.io/badge/Machine%20Learning-building-5B5BD6?style=flat-square" />
  <img alt="Multimodal AI" src="https://img.shields.io/badge/Multimodal%20AI-exploring-FF6B6B?style=flat-square" />
  <img alt="Computer Vision" src="https://img.shields.io/badge/Computer%20Vision-creating-0EA5E9?style=flat-square" />
</p>

## 🙂 a little about me

I'm **Nguyen Tran Khuong An**, an Applied AI Engineer with a Computer Science degree from the University of Information Technology (VNU-HCM). I'm interested in turning ideas from machine learning research into systems that actually work.

I enjoy the part of AI that sits between models and products: understanding how a model works, building the surrounding system, evaluating where it fails, and figuring out how to make the whole thing useful outside a notebook.

My interests currently sit around:

- 🤖 Machine Learning & Deep Learning
- 🧠 Large Language Models & Generative AI
- 👁️ Computer Vision
- 🔀 Multimodal AI
- 🔎 Information Retrieval & RAG
- ⚙️ AI Engineering & MLOps

I tend to follow a simple loop:

```
Understand → Build → Evaluate → Break → Improve
```

## 🧰 stuff I work with

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=python,cpp,pytorch,tensorflow,sklearn,fastapi,postgres,mongodb,redis,elasticsearch,docker,githubactions,aws,git,linux&perline=5" />
  </a>
</p>

<p align="center">
  <img alt="Hugging Face" src="https://img.shields.io/badge/Hugging%20Face-Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
  <img alt="OpenCV" src="https://img.shields.io/badge/OpenCV-Computer%20Vision-5C3EE8?style=flat-square&logo=opencv&logoColor=white" />
  <img alt="LangChain" src="https://img.shields.io/badge/LangChain-LLM%20Applications-1C3C3C?style=flat-square" />
  <img alt="LangGraph" src="https://img.shields.io/badge/LangGraph-Agents-1C3C3C?style=flat-square" />
  <img alt="RAG" src="https://img.shields.io/badge/RAG-Retrieval%20%2B%20Generation-10B981?style=flat-square" />
  <img alt="Vector DBs" src="https://img.shields.io/badge/Vector%20DBs-FAISS%20%C2%B7%20Milvus%20%C2%B7%20pgvector-F59E0B?style=flat-square" />
  <img alt="MLflow" src="https://img.shields.io/badge/MLflow-Experiment%20Tracking-0194E2?style=flat-square&logo=mlflow&logoColor=white" />
  <img alt="Airflow" src="https://img.shields.io/badge/Airflow-Pipelines-017CEE?style=flat-square&logo=apacheairflow&logoColor=white" />
</p>


## 🧠 the kind of things I build

### 🔎 [Multimodal Video Event Retrieval](https://github.com/kuongan/Event-Retrieval-System)

*Team lead (5 people)*

A search engine for finding specific events inside large video collections from a natural-language description. The hard part isn't embedding frames. It's that one signal is never enough: what's *seen*, what's *written* on screen, and what's *said* each catch different queries.

- **Pipeline:** keyframe extraction → OCR + ASR → multimodal embeddings from Vision-Language Models
- **Retrieval:** hybrid vector, lexical, and semantic search over Milvus, Elasticsearch, and MongoDB
- **Reranking:** this work published at SOICT 2025 and evaluated in the AI Challenge 2025

`PyTorch · Transformers · Milvus · Elasticsearch · MongoDB · Gemini`

### 👁️ [Low-Light Vehicle Enhancement & Detection](https://github.com/DatTran0509/Enhancing-and-Detecting-Vehicles-in-Low-Light-Conditions)

*Team lead (3 people)*

Detectors trained on daytime images fall apart at night. This project tests whether fixing the *image* first helps more than tuning the *detector*.

- Two-stage pipeline: **Zero-DCE** low-light enhancement → **YOLOv8** / **Faster R-CNN** detection
- Compared one-stage and two-stage detectors to trade off accuracy and speed
- Enhancing visibility before inference improved detection in low-light conditions

`PyTorch · OpenCV · YOLOv8 · Faster R-CNN · Zero-DCE`

### ⚙️ [Flight Query System](https://github.com/kuongan/sql-rag-system)

*Individual · [Demo](https://youtu.be/WDya8UZcTbA)*

A multi-agent system that lets people ask questions about flight data in plain language and get answers back as tables and charts.

- Natural language → SQL translation, orchestrated as a LangGraph agent workflow
- FAISS-based semantic retrieval to ground queries in the right schema and context
- Automated visualizations, served through a FastAPI backend and a Next.js frontend

`FastAPI · LangChain · LangGraph · SQLite · FAISS · Next.js · Tailwind`

> Also: a [Kolmogorov-Arnold Network (KAN) reproduction](https://github.com/kuongan/kan-reproduction). I reproduced the paper's formula-regression results, then compared KAN against MLPs on Titanic and MNIST.

## 🔬 research

**[Reading the Signs: A Graph-Based System for Multimodal Information Retrieval on Vietnamese Traffic Law](https://aclanthology.org/2025.vlsp-1.49/)**
*VLSP 2025 · 🥈 Top 2, Subtask 1: Multimodal Legal Retrieval*

A retrieval system that links traffic-sign images, legal text, and tabular data in a heterogeneous graph. It uses Grounding DINO and SigLIP to understand the signs, graph-guided search (BFS + dynamic top-k) to retrieve legal articles, and QwenVL / InternVL for visual question answering.

`Multimodal Learning · Information Retrieval · Knowledge Graphs · VQA`

**[From Discriminative Regions to Complete Masks: CAM–SAM Fusion for Weakly Supervised Semantic Segmentation](https://ieeexplore.ieee.org/document/11365118)**
*RIVF 2025*

Class Activation Maps only highlight the most discriminative part of an object. This work fuses CAMs with SAM through Semantic-Aware Prompting (SAP) to produce more complete pseudo-masks. It grew out of my undergraduate thesis, *Improving Class Activation Map for WSSS*, which used ViT/DeiT backbones for CAM and Mask2Former (Swin-L) for segmentation.

`Computer Vision · Weakly Supervised Learning · Vision Transformers · SAM`

<p align="center">
  <em>…and more.</em> See the full list of publications on
  <a href="https://scholar.google.com/citations?user=DSbVqkIAAAAJ&hl=en"><img alt="Google Scholar" src="https://img.shields.io/badge/Google%20Scholar-view%20all-4285F4?style=flat-square&logo=googlescholar&logoColor=white" align="center" /></a>
</p>

## 🏆 highlights

- 🎓 NVIDIA Jensen Huang Scholarship recipient
- 🥈 Top 2 Multimodal Legal Retrieval, VLSP 2025
- 🚀 Top 5 Southern Vietnam Google Developer Group on Campus Hackathon 2025 (healthcare assistant with medical tool calling)
- 📚 5× consecutive Academic Encouragement Scholarship

## 🧪 things I'm currently exploring

- Transformer architectures and their internals
- LLMs and efficient fine-tuning
- Retrieval-Augmented Generation
- Multimodal learning
- Computer Vision
- AI agents and tool-using systems
- Model evaluation and reliability
- Deploying ML systems beyond notebooks

## 📊 GitHub

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=kuongan&hide_border=true&theme=transparent" />
</p>

## 🤝 say hi
If you're building something interesting, feel free to reach out.

<p>
  <a href="https://www.linkedin.com/in/an-nguyen-tran-khuong/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://scholar.google.com/citations?user=DSbVqkIAAAAJ&hl=en"><img alt="Google Scholar" src="https://img.shields.io/badge/Google%20Scholar-research-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white" /></a>
  <a href="mailto:ankhuong.working@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-say%20hello-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>
