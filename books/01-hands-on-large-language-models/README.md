# Hands-On Large Language Models
### Language Understanding and Generation

| | |
|---|---|
| **Authors** | Jay Alammar, Maarten Grootendorst |
| **Publisher** | O'Reilly Media |
| **Published** | September 2024 (First Edition) |
| **ISBN** | 978-1-098-15096-9 |
| **Code & notebooks** | https://github.com/HandsOnLLM/Hands-On-Large-Language-Models |
| **Book page** | https://oreil.ly/hands_on_LLMs_1e |

> 🔗 To buy or read the book legally, visit the publisher's page (O'Reilly).
> The book file itself is not included in this repository.

---

## 🤔 What Is This Book?

A **visual, hands-on guide** to understanding and using large language models (LLMs).
Its philosophy is *intuition first*: you grasp each concept through illustrations and
examples, then run it in code. Nearly every concept has a figure, and all code runs on
**Google Colab** with a free GPU (T4, 16 GB VRAM).

One distinction runs through the whole book:

- **Representation models** (e.g., BERT): do not generate text; used for classification, embeddings, and search.
- **Generative models** (e.g., GPT): generate text.

## 👥 Who Is It For?

- Python programmers who want to get into LLMs
- Students and researchers in NLP and machine learning
- Engineers building RAG systems, chatbots, semantic search, or text clustering pipelines
- Anyone who wants to understand how Transformers and LLMs work under the hood

**Prerequisites:** Python programming experience and familiarity with basic machine learning.
No prior knowledge of PyTorch, TensorFlow, or generative modeling is needed. The book focuses on
intuition rather than mathematical derivations.

## 🎯 What Will You Learn?

- The history of Language AI: from bag-of-words and word2vec to attention and the Transformer
- Tokenization and embeddings
- The internal architecture of Transformers and how text is generated
- Text classification with representation and generative models
- Text clustering and topic modeling with BERTopic
- Prompt engineering and reasoning (chain-of-thought and more)
- LangChain: chains, memory, and agents
- Semantic search, reranking, and RAG
- Multimodal models (text + images) with CLIP and BLIP-2
- Creating and fine-tuning embedding models
- Fine-tuning generative models with LoRA/QLoRA and preference tuning with DPO

## 🧱 Book Structure

The book has three parts, and each chapter can be read independently.

---

### Part I: Understanding Language Models

**Chapter 1 — An Introduction to Large Language Models**
The history of Language AI: bag-of-words, word2vec, RNNs and attention, the "Attention Is All You Need" paper and the Transformer, encoder-only (BERT) and decoder-only (GPT) models. Also covers how LLMs are trained (pretraining and fine-tuning), applications, ethical considerations, open vs. proprietary models, and generating your first text with Phi-3.

**Chapter 2 — Tokens and Embeddings**
How text is split into tokens, a comparison of real tokenizers (BERT, GPT-2, GPT-4, StarCoder2, Galactica, Phi-3), word2vec and contrastive training, and building a song recommendation system with embeddings.

**Chapter 3 — Looking Inside Large Language Models**
The forward pass, token-by-token generation, the KV cache, the Transformer block (attention and feedforward layers), and recent improvements: grouped-query attention, Flash Attention, and RoPE.

---

### Part II: Using Pretrained Language Models

**Chapter 4 — Text Classification**
Sentiment classification of movie reviews (Rotten Tomatoes) with a task-specific model, with embeddings plus logistic regression, zero-shot classification, and with generative models (Flan-T5 and ChatGPT).

**Chapter 5 — Text Clustering and Topic Modeling**
The embedding → UMAP → HDBSCAN pipeline on ArXiv papers, then BERTopic with representation blocks (KeyBERTInspired, MMR, and LLM-generated labels).

**Chapter 6 — Prompt Engineering**
Choosing and controlling a generative model (temperature and top_p), prompt components, in-context learning, chain prompting, chain-of-thought, self-consistency, tree-of-thought, and output validation with constrained sampling (grammars).

**Chapter 7 — Advanced Text Generation Techniques and Tools**
With LangChain: loading quantized models, chains, conversation memory types (buffer, windowed, and summary), and agents using the ReAct framework.

**Chapter 8 — Semantic Search and Retrieval-Augmented Generation**
Dense retrieval, chunking, reranking, evaluation metrics (MAP and nDCG), RAG with API-based and local models, and advanced techniques: query rewriting, multi-query, multi-hop, query routing, and agentic RAG.

**Chapter 9 — Multimodal Large Language Models**
The Vision Transformer, multimodal embedding models (CLIP/OpenCLIP), and adding vision to generative models with BLIP-2 (image captioning and chatting about images).

---

### Part III: Training and Fine-Tuning Language Models

**Chapter 10 — Creating Text Embedding Models**
Contrastive learning, SBERT, loss functions (softmax, cosine similarity, MNR), Augmented SBERT, and unsupervised learning with TSDAE.

**Chapter 11 — Fine-Tuning Representation Models for Classification**
Fine-tuning BERT, freezing layers, few-shot classification with SetFit, continued pretraining with masked language modeling, and named-entity recognition (NER).

**Chapter 12 — Fine-Tuning Generation Models**
The three stages of LLM training, supervised fine-tuning, PEFT (adapters, LoRA, and QLoRA), evaluating generative models (benchmarks, leaderboards, and human evaluation), and preference tuning with reward models and DPO.

---

## 💻 Hardware and Software

- Easiest option: **Google Colab** (free T4 GPU)
- Running locally: an NVIDIA GPU with at least 16 GB of VRAM

```bash
conda create -n thellmbook python=3.10
conda activate thellmbook
git clone https://github.com/HandsOnLLM/Hands-On-Large-Language-Models
cd Hands-On-Large-Language-Models
pip install -r requirements.txt
```

Some examples require API keys (OpenAI, Cohere, and Hugging Face for Llama 2).

## ✍️ My Take

> Fill this section in yourself: your personal experience, favorite chapters, strengths and weaknesses, and a suggested reading path.

## 🔗 Resources

- Official code repository: https://github.com/HandsOnLLM/Hands-On-Large-Language-Models
- Book page: https://oreil.ly/hands_on_LLMs_1e
