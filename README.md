## 🌸 InnerBloom — AI Mental Health Support Chatbot

**InnerBloom** is an end-to-end AI-powered mental health support chatbot built using **Mistral-7B-Instruct** and fine-tuned with **LoRA (Low-Rank Adaptation)**.
The project combines **instruction fine-tuning**, **retrieval-augmented generation (RAG)**, and a **Gradio-based conversational UI** to provide empathetic, context-aware responses in a safe and user-friendly environment.

---

## 🚀 Key Features

* **LoRA Fine-Tuning (4-bit)**
  Efficient fine-tuning of Mistral-7B using PEFT and BitsAndBytes, enabling training on limited GPU resources.

* **Instruction-Tuned Dataset Pipeline**
  Custom JSON → JSONL conversion for supervised instruction tuning with masked prompt tokens.

* **Retrieval-Augmented Generation (RAG)**
  Uses **ChromaDB** with **Sentence-Transformers embeddings** to retrieve relevant knowledge from datasets and documents.

* **Memory-Efficient Inference**
  Automatic device mapping, 4-bit quantization, and CPU/GPU offloading for smooth inference on Kaggle.

* **Interactive Chat Interface**
  A clean, styled **Gradio chat UI** designed as a safe space for emotional support and conversation.

* **Modular & Production-Ready**
  Includes training scripts, inference loaders, dataset processing, vector storage, and optional FastAPI integration.

---

## 🧠 Architecture Overview

* **Base Model:** `mistralai/Mistral-7B-Instruct-v0.2`
* **Fine-Tuning:** LoRA adapters (PEFT)
* **Quantization:** 4-bit (BitsAndBytes)
* **Vector Store:** ChromaDB
* **Embeddings:** all-MiniLM-L6-v2
* **UI:** Gradio
* **Deployment Ready:** FastAPI compatible

---

## 📂 Project Pipeline

1. Convert raw dataset to instruction-tuning JSONL format
2. Store dataset knowledge in Chroma vector database
3. Tokenize and prepare supervised fine-tuning data
4. Train LoRA adapters on Mistral-7B (4-bit)
5. Load base model + LoRA adapters for inference
6. Serve responses via Gradio chat interface

---

## 🎯 Use Case

InnerBloom is designed to demonstrate how **large language models can be adapted for empathetic, domain-specific conversations** while remaining efficient, scalable, and deployable on limited hardware.
It is suitable for educational, research, and proof-of-concept applications in **AI-assisted mental health support**.

---

## ⚠️ Disclaimer

This project is intended for **research and educational purposes only** and does **not replace professional mental health care**.




🖥 User Interface

The chatbot features a clean and calming web interface built with Gradio, designed to provide a safe and comfortable user experience.
It includes a real-time chat window, message input field, send and clear chat buttons, and a visually soothing theme that aligns with the project’s mental health focus.
<img width="1865" height="920" alt="image" src="https://github.com/user-attachments/assets/acb3c0bf-7cb3-4980-98b9-bceadce1ac3c" />

