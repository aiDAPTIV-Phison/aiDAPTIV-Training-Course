<div align="center">

<a href="https://www.phison.com/en/aidaptiv-plus-ai-data-storage-solution"><picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/atp224/aiDAPTIV-Training-Course/blob/e7303bc3326fa84a07add8e6bc9ba384f3a53431/assets/dark_logo.png">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/atp224/aiDAPTIV-Training-Course/blob/e7303bc3326fa84a07add8e6bc9ba384f3a53431/assets/light_logo.png">
    <img alt="aiDAPTIV+ logo" src="https://github.com/atp224/aiDAPTIVTestPage/blob/main/assets/aiDAPTIV_logo.jpg?raw=true" height="110" style="max-width: 100%;">
  </picture></a>

# aiDAPTIV+ Training Course – Hands-On LLM Fine-Tuning

</div>

Learn how to fine-tune large language models (LLMs) locally using **aiDAPTIV+** with both the **Pro Suite Graphical User Interface** and the **Command Line Interface**. This repository contains all lesson materials, datasets, code examples, and project files to learn aiDAPTIV+.

---

## 📚 About This Course
This hands-on curriculum is designed to teach you how to:
- Fine-tune LLMs on your own hardware or a provided remote AI Training PC (AITPC).
- Optimize GPU VRAM usage with **aiDAPTIVCache**.
- Use both GUI and CLI workflows for training and inference.
- Apply fine-tuning to real-world datasets such as company handbooks or public figure transcripts.

The course includes about **2 hours of recorded, follow-along video content**, but the full experience takes around **12 hours to complete**.  
Most of that time is spent running fine-tuning jobs, so you don’t need to stay at your computer while training is in progress.  

Whether you’re a developer, researcher, or student, you’ll gain practical skills to run on-prem AI cost-efficiently and securely.

---

## 🚀 Getting Started

### Prerequisites
- [aiDAPTIV+ Installed](https://github.com/atp224/aiDAPTIVTestPage/tree/main/Page_Sections/Installation)
- [Access to an AI Training PC (AITPC)](https://docs.google.com/forms/d/e/1FAIpQLSd1KLGisv-xU9KIc8ZPQBIBEfbS1VCW16qxCCXe-5_ZGfcgxg/viewform) either your own system with aiDAPTIV+ installed **or** remote access to a provided AITPC

### Setup
```bash
git clone https://github.com/aiDAPTIV-Phison/aiDAPTIV-Training-Course
cd aiDAPTIV-Training-Course
```

---

## Lessons

| Lesson Number | Topic | Lesson Grouping | Learning Objectives | Linked Lesson |
| :-----------: | :------------------------------: | :--------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------: |
| 01 | Welcome & Introduction | [Introduction](1-Introduction/README.md) | Overview of the aiDAPTIV+ platform, course structure, and how to get started. | [lesson](1-Introduction/01-welcome/README.md) [video](https://youtu.be/OtenwmjlDFs) |
| 02 | Accessing the AI Training PC | [Introduction](1-Introduction/README.md) | Learn how to request, connect to, and work with the remote AITPC for course exercises. | [lesson](1-Introduction/02-accessing-the-AI-Training-PC/README.md) [video]() |
| 03 | Fine-Tuning via Pro Suite GUI | [GUI Based](2-GUI-Based/README.md) | Use the aiDAPTIV+ Pro Suite GUI to fine-tune a custom LLM using the Phison Employee Handbook dataset. | [lesson](2-GUI-Based/03-fine-tune/README.md) [video](https://youtu.be/bvzh1CztTgU) |
| 04 | Instruction Fine-Tuning | [CLI Based](3-CLI-Based/README.md) | Learn how to fine-tune a model on instruction–response datasets for more structured outputs. | [lesson](3-CLI-Based/04-instruction-fine-tuning/README.md) [video](https://youtu.be/470m1BNNEyY) |
| 05 | Speaking Style Model | [CLI Based](3-CLI-Based/README.md) | Fine-tune an LLM to adapt its output style for different tones, audiences, and communication needs. | [lesson](3-CLI-Based/05-speaking-style-model/README.md) [video](https://youtu.be/bvzh1CztTgU) |
| 06 | RAFT Dataset Generation | [CLI Based](3-CLI-Based/README.md) | Generate retrieval-augmented datasets to improve factual grounding and domain specialization. | [lesson](3-CLI-Based/06-RAFT-Dataset-Generation/README.md) [video](https://youtu.be/Q3e-Q05ccJ8) |
| 07 | LLM as a Judge | [CLI Based](3-CLI-Based/README.md) | Use LLMs to evaluate and grade outputs from other models with rubrics. | [lesson](3-CLI-Based/07-LLM-as-a-judge/README.md) [video](https://youtu.be/YnrOuSRJum8) |
| 08 | Vision Function Calling | [CLI Based](3-CLI-Based/README.md) | Explore how Vision-Language Models (VLMs) can analyze images and trigger structured functions. | [lesson](3-CLI-Based/08-vision-function-calling-model/README.md) [video]() |




---

## 🤝 Contributing
Feedback and improvements are welcome. Please open an issue or submit a pull request if you find bugs or have suggestions.

