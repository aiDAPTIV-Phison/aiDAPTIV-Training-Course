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

## Lessons

|![ Sketchnote placeholder ](./sketchnotes/00-Roadmap.png)|
|:---:|
| aiDAPTIV+ Training Course: Roadmap |

| Lesson Number | Topic | Lesson Grouping | Learning Objectives | Linked Lesson | Author |
| :-----------: | :------------------------------: | :--------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------: | :----: |
| 01 | Welcome & Introduction | [Introduction](1-Introduction/README.md) | Overview of the aiDAPTIV+ platform, course structure, and how to get started. | [lesson](1-Introduction/01-welcome/README.md) | Aaron Pham |
| 02 | Accessing the AI Training PC | [Introduction](1-Introduction/README.md) | Learn how to request, connect to, and work with the remote AITPC for course exercises. | [lesson](1-Introduction/02-remote-aitpc/README.md) | Aaron Pham |
| 03 | Fine-Tuning via Pro Suite GUI | [GUI Based](2-GUI-Based/README.md) | Use the aiDAPTIV+ Pro Suite GUI to fine-tune a custom LLM using the Phison Employee Handbook dataset. | [lesson](2-GUI-Based/03-pro-suite-handbook/README.md) | Aaron Pham |
| 04 | CLI Fine-Tuning: Speaking Style Model | [CLI Based](3-CLI-Based/README.md) | Fine-tune an LLM to mimic a public figure’s speaking style using aiDAPTIV+ CLI tools. | [lesson](3-CLI-Based/04-speaking-style/README.md) | Aaron Pham |
| 05 | CLI Fine-Tuning: Vision Function Calling Model | [CLI Based](3-CLI-Based/README.md) | Build and fine-tune an LLM capable of vision-based function calling through the CLI workflow. | [lesson](3-CLI-Based/05-vision-function-calling/README.md) | Aaron Pham |

---

## 🤝 Contributing
This repository is primarily for learners of the Udemy course, but feedback and improvements are welcome. Please open an issue or submit a pull request if you find bugs or have suggestions.

---

## 📜 License
This course material is licensed under the MIT License. You are free to use, modify, and share, but attribution is appreciated.
