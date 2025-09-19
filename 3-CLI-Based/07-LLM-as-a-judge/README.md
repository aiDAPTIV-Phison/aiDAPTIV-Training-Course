# LLM as a Judge

**Why this matters:**  
Traditional evaluation methods (like [BLEU](https://huggingface.co/spaces/evaluate-metric/bleu) or [string matching](https://huggingface.co/spaces/evaluate-metric/exact_match)) can’t tell if an answer is *actually* correct, they only check surface overlap. This is a big problem when detecting **hallucinations**, since a response can look different but still be valid, or look similar but be misleading.  
Using **LLMs as judges** solves this by applying reasoning and context awareness to evaluation, leading to more **accurate, meaningful, and reliable** assessments of model outputs.

In this lesson, you’ll learn how to use **LLMs as evaluators** to detect hallucinations in model outputs. Instead of relying on string similarity metrics, LLM-as-a-Judge leverages reasoning to score responses more accurately.  

<p align="center">
  <a href="https://youtu.be/YnrOuSRJum8" target="_blank">
    <img src="https://github.com/aiDAPTIV-Phison/aiDAPTIV-Training-Course/blob/e60ff9d6c3597c4d2f8de5ea3f2bef1f96b82fdd/assets/LLM_as_a_Judge.png" alt="LLM-as-a-Judge Video" width="600"/>
  </a>  
  <br>
  ▶️ *Click the image above to watch the video on YouTube.*
</p>

---

## What is LLM-as-a-Judge?

Consider a customer service bot asked:  
**Q:** “What is your return policy?”  
- Correct answer: “You can return items within 30 days of purchase.”  
- Bot’s answer: “You can return items within 30 days.”  

A string comparison metric may incorrectly mark this as *wrong*. Instead, an **LLM-as-a-Judge** can evaluate whether the answer is essentially correct and faithful.  

This approach:  
- Goes beyond surface-level text matching.  
- Captures meaning, reasoning, and context.  
- Provides structured judgments (scores, reasoning, classifications).  

---

## Lesson Overview

In this notebook, we will:  
1. Set up an **LLM inference service**.  
2. Explore and prepare the **CoQA dataset**.  
3. Add **hallucinated answers** for testing.  
4. Create and compare multiple **LLM-as-a-Judge evaluators**.  
5. Review next steps for refinement and experimentation.  

---

## 1. Setting up the Inference Service

- Download the **LLaMA 3.1–8B model** from Hugging Face.  
- Store the model checkpoint locally.  
- Run a **Docker container** to serve the inference API.  

We’ll use helper functions to:  
- Save the container ID.  
- Run the container.  
- Stop it when finished.  

---

## 2. Exploring the Dataset

We use the **CoQA dataset**, which contains passages, questions, and answers.  
- Flatten into `(passage, question, answer)` tuples.  
- Note: Since CoQA is public, there’s a chance parts may be memorized by LLMs. For production, you should evaluate with **private data**.  

---

## 3. Adding Hallucinations

To test robustness, we’ll generate **hallucinated answers** by asking an LLM to respond confidently without looking at the passage.  
- This lets us compare real answers vs. hallucinations.  
- Provides training and evaluation material for our judges.  

---

## 4. Creating Evaluators

We experiment with multiple evaluation styles:  

### 4.1 Numeric Rater  
Ask the LLM to rate an answer on a scale (e.g., **1–10**).  
- ✅ Easy to implement.  
- ❌ Lacks reasoning, may be inconsistent.  

### 4.2 Adding Reasoning (Chain of Thought)  
Ask the LLM to explain *why* it gave the score.  
- Provides interpretability.  
- Can improve consistency.  

### 4.3 Classification-Based Judging  
Instead of numeric ratings, specify criteria (e.g., **Correct / Partially Correct / Incorrect**).  
- Guides the model toward the **hallucinations of interest**.  
- Produces more **reliable structured results**.  

---

## 5. Next Steps

After setting up your evaluator, consider:  
- Testing on your **own private data**.  
- Comparing different models (e.g., o1 vs smaller fine-tuned models).  
- Using **few-shot prompting** for subjective judgments.  
- Rigorously measuring impact across datasets.  

---

## Review & Self Study

This lesson covered:  
- Why **LLM-as-a-Judge** is better than string metrics.  
- How to set up an inference service.  
- Preparing CoQA with hallucinations for testing.  
- Comparing different judging strategies.  

**For further study:**  
- [Evaluation Metrics](https://www.geeksforgeeks.org/machine-learning/metrics-for-machine-learning-model/m)  
- [OpenAI Evaluation Framework](https://platform.openai.com/docs/guides/evals)  
- [Evaluation Best Practices](https://huggingface.co/docs/evaluate/index)  

---

## Assignment

**LLM-as-a-Judge Demo** – build your own evaluator.  
- Pick a dataset with QA pairs.  
- Add at least 5 hallucinated answers.  
- Implement at least **two judging methods** (numeric + classification).  
- Compare results and reflect on strengths/weaknesses.  
