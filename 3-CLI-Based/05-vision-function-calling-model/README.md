# Vision Function Calling

In this lesson you will learn how modern **Vision-Language Models (VLMs)** can not only describe images but also **call functions** based on what they see. By combining **OCR-like perception** with structured reasoning and APIs, we can unlock powerful multimodal workflows.

[![Intro Video](images/video-prob-and-stats.png)](https://youtu.be/Z5Zy85g4Yjw)

We will demonstrate this using the **Qwen2.5-VL-3B-Instruct** model and two real-world examples:
1. Simulating a customer service assistant to handle delivery exception screenshots.  
2. Analyzing an organizational chart to extract employee information into structured data.  

---

## What are Vision-Language Models?

Traditional **OCR (Optical Character Recognition)** tools focus only on extracting text from an image.  
Vision-Language Models go further:
- They understand **images holistically** (objects, layout, context).  
- They can **reason** about what they see (e.g., “the package is marked as delayed”).  
- They combine this reasoning with **natural language capabilities**.  

Examples of popular VLMs include **Qwen-VL**, **LLaVA**, and **GPT-4o**.

---

## What is Function Calling?

Function calling allows the model to go beyond free-form text output. Instead, it can **trigger structured actions** such as:  
- Returning **JSON data**.  
- Invoking APIs (e.g., a tracking system or HR database).  
- Acting as a bridge between **AI understanding** and **software automation**.  

> ✅ Think of function calling as giving the AI “tools” to respond in ways a program can use directly, rather than just natural language.

---

## Lesson Overview

In this notebook, we will:
- Install and configure the **Qwen2.5-VL-3B-Instruct** model with Docker + vLLM.  
- Import necessary libraries and set up helper functions.  
- Download a sample dataset of images (delivery screenshots + org charts).  
- Run two example workflows:  
  1. **Customer service assistant** – interpret a delivery issue screenshot and produce structured support actions.  
  2. **Org chart analyzer** – extract employee names/roles and return them in structured JSON.  

---

## Example 1: Customer Service Assistant

We simulate a customer support workflow:
- Input: an image of a delivery exception notice.  
- Model task: identify the issue and recommend the next step.  
- Output: structured response (e.g., `{"action": "reschedule_delivery", "customer_id": 12345}`).

This shows how VLMs can **combine vision and reasoning** to automate business processes.

---

## Example 2: Analyzing an Org Chart

We pass in an organizational chart:
- Input: an image with boxes showing employee names/roles.  
- Model task: extract structured metadata.  
- Output: JSON containing each employee’s name and role.

This workflow demonstrates how **visual documents** can be converted into machine-readable data for HR or database systems.

---

## 🚀 Challenge

Try extending this notebook by:
- Testing with your own delivery screenshots.  
- Passing in other types of documents like invoices, receipts, or ID cards.  
- Writing a custom function schema and having the model call it.  

---

## [Post-lecture quiz](#)

---

## Review & Self Study

This lesson showed how to combine **OCR, image understanding, and function calling** into a single workflow.  
For further study:  
- [OpenAI Function Calling docs](https://platform.openai.com/docs/guides/function-calling)  
- [Qwen-VL GitHub](https://github.com/QwenLM/Qwen-VL)  
- Explore other multimodal frameworks like [LLaVA](https://llava-vl.github.io/)  

---

## Assignment

**Vision Function Calling Demo** – build a new example of your own using this notebook.  
- Pick an image type (e.g., receipt, chart, report).  
- Design a function schema that makes sense for your data.  
- Run inference and capture the structured output.  
