# aiDAPTIV+ Training Course – Hands-On LLM Fine-Tuning

Learn how to fine-tune large language models (LLMs) locally using **aiDAPTIV+** with both the **Pro Suite Graphical User Interface** and the **Command Line Interface**. This repository contains all lesson materials, datasets, code examples, and project files to learn aiDAPTIV+.

---

## 📚 About This Course
This hands-on curriculum is designed to teach you how to:
- Fine-tune LLMs on your own hardware or a provided remote AI Training PC (AITPC).
- Optimize GPU VRAM usage with **aiDAPTIVCache**.
- Use both GUI and CLI workflows for training and inference.
- Apply fine-tuning to real-world datasets such as company handbooks or public figure transcripts.

Whether you’re a developer, researcher, or student, you’ll gain practical skills to run on-prem AI cost-efficiently and securely.

---

## 🗂 Repository Structure
```
/lessons
    /pro-suite-gui
    /cli
/projects
    /handbook-chatbot
    /speaking-style-model
/data
    /sample-datasets
/scripts
    fine_tune.py
    inference.py
README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.10+
- PyTorch installed (CUDA-enabled recommended)
- aiDAPTIV+ Pro Suite or CLI installed (instructions in course)
- Access to an aiDAPTIVCache SSD or AITPC (optional but recommended)

### Setup
```bash
git clone https://github.com/yourusername/aidaptiv-plus-training.git
cd aidaptiv-plus-training
pip install -r requirements.txt
```

---

## 📂 Lessons & Projects
- **Lesson 1** – Introduction to aiDAPTIV+ and VRAM Optimization
- **Lesson 2** – Fine-Tuning with the Pro Suite GUI
- **Lesson 3** – Fine-Tuning with the CLI
- **Project: Company Handbook Chatbot**
- **Project: Public Figure Speaking Style Model**

---

## 🤝 Contributing
This repository is primarily for learners of the Udemy course, but feedback and improvements are welcome. Please open an issue or submit a pull request if you find bugs or have suggestions.

---

## 📜 License
This course material is licensed under the MIT License. You are free to use, modify, and share, but attribution is appreciated.
