# 🦥 Unsloth Fine-Tune Hub (Colab Edition)

A comprehensive Colab-based interface designed to simplify and simulate the fine-tuning of popular language models using the [Unsloth](https://github.com/unslothai/unsloth) library and [Gradio](https://www.gradio.app/) UI components. Ideal for experimentation, educational demos, and prototyping scalable LLM pipelines.

Built and curated by [Raghav](https://github.com/Raghav0079), this tool bridges cutting-edge optimization with user-friendly interaction.

---

## ✨ Core Features

- 🔍 **Model Selection**  
  Fine-tune across major LLM architectures: **LLaMA-2**, **Mistral**, and **Falcon**, all integrated via dropdown for easy selection.

- 📊 **Hyperparameter Control**  
  Dynamically adjust key parameters like **learning rate** and **batch size** — no code edits required.

- 📁 **Custom Dataset Upload**  
  Accepts training files in **.csv** and **.jsonl** format with auto-validation and status feedback.

- 🧪 **Simulated Fine-Tuning Preview**  
  See how your settings would be applied, ideal for understanding workflows before jumping into compute-heavy training.

- 📈 **Roadmap Features**  
  Coming soon: Full integration of Unsloth’s training APIs and **WandB logging** for experiment tracking.

---

## 🚀 Quickstart Guide

### 1. Open in [Google Colab](https://colab.research.google.com/)
> Make sure you have GPU runtime enabled (under *Runtime > Change runtime type*)

### 2. Run Setup Cells Sequentially
Each cell is clearly labeled:
- Install dependencies: `gradio`, `transformers`, `unsloth`, `accelerate`, `datasets`
- Import all relevant libraries
- Check GPU availability
- Define the placeholder `fine_tune()` function
- Build Gradio app interface
- Launch Gradio app (final cell provides **public shareable URL**)

### 3. Configure via Gradio UI
Once launched:
- Select your base LLM from dropdown
- Enter preferred learning rate and batch size
- Upload `.csv` or `.jsonl` dataset
- Click **🚀 Launch Fine-Tune**
- Status updates will stream directly in-app

---

## 🧠 Under the Hood

- **Framework**: Powered by Unsloth for efficiency and fast adapter-based tuning
- **Interface**: Gradio provides an accessible way to interact with hyperparameters without diving into backend code
- **Notebook Structure**: Modular cell layout enables easy adaptation into other training scripts or extensions like real-time training or leaderboard comparison

This project aims to lower the barrier to entry for LLM training by offering a sandbox-style simulator before diving into actual model weight updates.

---

## 🧩 Planned Enhancements

| Feature              | Status        | Notes |
|----------------------|---------------|-------|
| ✅ Gradio UI          | Complete       | Fully functional |
| 🔄 Real Unsloth Tuning | In Progress   | Hook into `UnslothTrainer()` |
| 🔍 WandB Integration   | Pending        | Track fine-tune metrics live |
| 🔬 Evaluation Suite   | Proposed       | Add BLEU, ROUGE, perplexity reports |

---

## 🛠️ Contributing

Whether you're refining the UI, adding training logic, or porting to other platforms — pull requests are welcome!

1. Fork the repo
2. Create a feature branch
3. Document your changes clearly
4. Submit your PR with a descriptive commit message

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).  
You're free to use it commercially, modify it, or build upon it.

---

## 📌 Acknowledgements

- [Unsloth](https://github.com/unslothai/unsloth) for streamlined LLM training tools
- [Gradio](https://www.gradio.app/) for interactive UI components
- [HuggingFace](https://huggingface.co/) for providing open access model weights

---

## Notebook Link

https://colab.research.google.com/drive/1f6CyiVTY-p3k7NWmLOgsUsZhemxcP87r?usp=drive_link
