# Work In Progress - Vision Function Calling

**Why this matters:**  
Traditional Vision-Language Models (VLMs) can describe what they see, but they usually stop at captions or Q&A. Real-world applications often need **action**, not just description, like extracting numbers from receipts, scheduling from a whiteboard snapshot, or triggering workflows from diagrams.  
By teaching VLMs to **call functions** based on visual input, we bridge perception with automation, enabling **multimodal agents** that can reason, act, and integrate directly into business or research pipelines.

In this lesson, you will learn how modern **Vision-Language Models (VLMs)** can not only describe images but also **call functions** based on what they see. By combining **OCR-like perception** with structured reasoning and APIs, we can unlock powerful multimodal workflows.

<p align="center">
  <a href="https://youtu.be/UFYZY9aUPvk" target="_blank">
    <img src="https://github.com/aiDAPTIV-Phison/aiDAPTIV-Training-Course/blob/e60ff9d6c3597c4d2f8de5ea3f2bef1f96b82fdd/assets/Vision_Function_Calling.png" alt="Vision Function Calling Video" width="600"/>
  </a>  
  <br>
  ▶️ *This Video Is Currently being Recorded*
</p>

---

## What are Vision-Language Models?

Traditional **OCR (Optical Character Recognition)** tools focus only on extracting text from an image.  
Vision-Language Models go further:  
- Understand **images holistically** (objects, layout, context).  
- **Reason** about what they see (e.g., recognizing that if a package label shows a delivery date earlier than today, the package must be delayed).  
- Combine perception with **natural language capabilities**.  

Popular VLMs include **Qwen-VL**, **LLaVA**, and **GPT-4o**.

---

## What is Function Calling?

Function calling allows the model to go beyond free-form text output. Instead, it can **trigger structured actions** such as:  
- Returning **JSON data**.  
- Invoking APIs (e.g., tracking systems, HR databases).  
- Acting as a bridge between **AI understanding** and **software automation**.  

> ✅ Think of function calling as giving the AI “tools” to respond in ways a program can use directly, not just natural language.

---

## Lesson Overview

In this notebook, we will:  
1. Install and configure the **Qwen2.5-VL-3B-Instruct** model with Docker + vLLM.  
2. Import necessary libraries and helper functions.  
3. Download a sample dataset of delivery exception screenshots.  
4. Run a real-world workflow:  
   - **Customer Service Assistant** – interpret a delivery issue screenshot and generate structured support actions.  

---

## Example: Customer Service Assistant

We simulate a **customer support workflow**:  
- **Input:** an image of a delivery exception notice.  
- **Task:** identify the issue and recommend the next step.  
- **Output:** structured JSON (e.g., `{"action": "reschedule_delivery", "customer_id": 12345}`).  

This demonstrates how VLMs can **combine vision and reasoning** to automate real-world processes.

---

## Review & Self Study

This lesson showed how to combine **OCR, image understanding, and function calling** into a single workflow.  

For further study:  
- [OpenAI Function Calling Docs](https://platform.openai.com/docs/guides/function-calling)  
- [Qwen-VL GitHub](https://github.com/QwenLM/Qwen-VL)  
- Explore multimodal frameworks like [LLaVA](https://llava-vl.github.io/)  

---

## Assignment

**Vision Function Calling Demo** – create your own example using this notebook.  
- Choose an image type (e.g., receipt, chart, report).  
- Design a function schema that fits your data.  
- Run inference and capture the structured output.  
