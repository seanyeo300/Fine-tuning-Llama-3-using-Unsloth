<h1>Fine-tuning-LLaMA-3-using-Unsloth</h1>

 <h2>Description</h2>
This repository documents my learning journey for fine-tuning LLaMA 3. Feel free to follow along using the curriculum provided.

<br />

## 🧠 Planned Curriculum: LLM Fine-tuning with LLaMA 3 + Unsloth

This section outlines my evolving curriculum for mastering LLM fine-tuning. It is structured progressively, from foundational concepts to advanced techniques, with a hands-on emphasis using the [Unsloth](https://github.com/unslothai/unsloth) framework and Meta's LLaMA 3 models.

---

### 📘 Phase 1: Foundations of LLMs and Fine-tuning

- [ ] Understand the Transformer architecture (Vaswani et al.)
- [ ] Review LLaMA 1/2/3 architectures (differences, improvements)
- [ ] Introduction to language modelling objectives (causal LM, MLM)
- [ ] Overview of fine-tuning vs instruction tuning vs RLHF
- [ ] Learn about parameter-efficient fine-tuning (PEFT) and LoRA

---

### 🔧 Phase 2: Setting Up the Fine-tuning Stack

- [ ] Environment setup (CUDA, PyTorch, Transformers, Unsloth)
- [ ] Familiarise with Unsloth's LLaMA 3 API and model loading
- [ ] Tokenizer and data preprocessing pipeline
- [ ] Understand memory usage, model quantisation (4-bit/8-bit)

---

### 🧪 Phase 3: Basic Fine-tuning

- [ ] Fine-tune LLaMA 3 using small datasets (e.g. Alpaca format)
- [ ] Use LoRA with Unsloth for efficient training
- [ ] Evaluate using perplexity and qualitative completions
- [ ] Save and resume training from checkpoints

---

### 🧭 Phase 4: Instruction and Chat Fine-tuning

- [ ] Understand chat templates (e.g. `chatml`, `alpaca`, `zephyr`)
- [ ] Curate or format instruction-tuning datasets (e.g. ShareGPT, OpenHermes)
- [ ] Evaluate model responses using prompt-response format
- [ ] Apply techniques for avoiding mode collapse / overfitting

---

### 🧠 Phase 5: Advanced Topics

- [ ] Data curriculum learning (easy-to-hard instance ordering)
- [ ] Custom reward models and early stopping heuristics
- [ ] Multi-turn conversation alignment
- [ ] Multi-objective fine-tuning (e.g. factuality + helpfulness)

---

### ⚙️ Phase 6: Experiment Tracking and Optimisation

- [ ] Integrate with Weights & Biases or MLflow
- [ ] Profile memory and compute usage
- [ ] Hyperparameter tuning strategies (batch size, lr, scheduler)
- [ ] Ablation studies on LoRA ranks, dataset size, prompt formats

---

### 📤 Phase 7: Deployment and Sharing

- [ ] Convert and quantise model for inference (GGUF, ONNX, etc.)
- [ ] Serve model using vLLM or Text Generation Inference
- [ ] Create Gradio/HF Spaces demo
- [ ] Publish LoRA adapters to Hugging Face Hub

---

_This roadmap is continuously evolving. Contributions, suggestions, and corrections are welcome._



<h2>Languages and Utilities Used</h2>

- <b>Python >=3.9; <=3.12  </b> 
- <b>Unsloth</b>

Installation instructions for unsloth on Windows can be found [here](https://docs.unsloth.ai/get-started/installing-+-updating/windows-installation)

<h2>Environments Used </h2>

- <b>Windows 11</b> (Pro)



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
