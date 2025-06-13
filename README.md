# Fine-tuning LLaMA 3.1 Using Unsloth for Legal Domain Specialisation

## 📄 Description

This repository documents my ongoing work in adapting Meta’s LLaMA 3.1 8B model for domain-specific applications in Singaporean law. It builds upon and extends the excellent work from [`xuyangbocn/LLM-RAG-singapore-lawyer`](https://github.com/xuyangbocn/LLM-RAG-singapore-lawyer), which establishes a RAG pipeline for statute-based question answering.

My objectives include:

- Specialising the embedding model via LoRA fine-tuning using [Unsloth](https://github.com/unslothai/unsloth)
- Aligning the model outputs to legal standards through Reinforcement Learning with Human Feedback (RLHF) in collaboration with a professional lawyer
- Deploying an offline-ready LLM for legal document summarisation and retrieval

---

## 🧠 Project Scope and Roadmap

<details>
<summary><strong>🚀 Project Phases</strong></summary>

### ✅ Phase 0: Baseline RAG Framework (Completed)

- ✔️ Investigated and adapted the `LLM-RAG-singapore-lawyer` architecture
- ✔️ Performed chunking and metadata tagging of legal statutes (PDFs)
- ✔️ Developed an initial RAG pipeline for legal QA using `LangChain`, `FAISS`, and `OpenChat`

---

### ⚙️ Phase 1: Domain-Specific Embedding Fine-tuning (In Progress)

- ❌ Prepare legal-specific contrastive data (e.g., semantically similar/dissimilar statute pairs)
- ❌ Fine-tune LLaMA 3.1 8B embeddings using LoRA via Unsloth
- ❌ Use quantised training (4-bit QLoRA) for efficient compute usage
- ❌ Evaluate domain specialisation using retrieval recall and legal topic clustering

---

### 🧑‍⚖️ Phase 2: RLHF with Legal Expert

- ❌ Collect human preference data on model completions from a practising lawyer
- ❌ Train a reward model to reflect legal accuracy, helpfulness, and clarity
- ❌ Apply PPO or DPO for alignment with legal preferences
- ❌ Evaluate using legal benchmarks and human qualitative assessments

---

### 🧪 Phase 3: Experimental Improvements (Planned)

- ❌ Investigate data curriculum learning for legal tasks (e.g., by statute complexity)
- ❌ Explore multi-turn dialogue alignment in legal consultations
- ❌ Test multi-objective RLHF with factuality and compliance scores

---

### 📤 Phase 4: Deployment

- ❌ Convert and quantise the model (GGUF/ONNX) for offline inference
- ❌ Integrate with lightweight web UI (e.g., Gradio)
- ❌ Package as a containerised app with offline RAG + inference capabilities

</details>

---

## 🛠 Languages and Frameworks

- **Python**: >= 3.9 and <= 3.12  
- **Unsloth** for efficient LoRA fine-tuning  
- **LangChain**, **FAISS**, **HuggingFace Transformers**
- **PyTorch**, **PEFT**, **RLHF tooling (TRL/DPO)**

> Note: Unsloth installation on Windows is documented [here](https://docs.unsloth.ai/get-started/installing-+-updating/windows-installation)

---

## 💻 Development Environment

- **Operating System**: Windows 11 Pro  
- **Target Hardware**: Consumer-grade GPU (8-24 GB VRAM) or cloud-based A100s for RLHF

---

## 🔗 Credits and References

- [LLM-RAG-singapore-lawyer](https://github.com/xuyangbocn/LLM-RAG-singapore-lawyer)
- [Unsloth](https://github.com/unslothai/unsloth)
- [Hugging Face PEFT](https://github.com/huggingface/peft)
- [TRL (Transformers Reinforcement Learning)](https://github.com/huggingface/trl)

---

_This repository is maintained monthly and may not reflect the latest developments and updates. Please contact the author for the latest discussions. Feedback, suggestions, and collaborations are welcome._
