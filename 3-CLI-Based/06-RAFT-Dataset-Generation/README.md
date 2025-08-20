# RAFT Dataset Generation

**Why this matters:**  
Large Language Models (LLMs) are powerful, but they often struggle with **domain-specific accuracy** and can generate **hallucinations** when asked about specialized topics. Traditional fine-tuning helps, but it doesn’t explicitly teach the model how to use external knowledge.  
**Retrieval-Augmented Fine-Tuning (RAFT)** solves this by combining fine-tuning with retrieval, letting the model not only access the right context but also *learn from retrieval-enriched data*. This results in models that are more **fact-grounded, accurate, and tailored** to your domain.

In this lesson, you will learn how to generate datasets for **Retrieval-Augmented Fine-Tuning (RAFT)**. RAFT extends Retrieval-Augmented Generation (RAG) by not only pulling relevant external knowledge into model responses, but also **fine-tuning models on retrieval-enriched data** to improve accuracy, factual grounding, and domain specialization.  


<p align="center">
  <a href="https://youtu.be/Q3e-Q05ccJ8" target="_blank">
    <img src="https://github.com/atp224/aiDAPTIV-Training-Course/blob/main/assets/RAFT_Dataset_Generation.png" alt="RAFT Dataset Generation" width="600"/>
  </a>  
  <br>
  ▶️ *Click the image above to watch the video on YouTube.*
</p>

---

## What is RAFT?

**Retrieval-Augmented Fine-Tuning (RAFT)** is a method to improve LLM performance by:  
1. Retrieving relevant documents from an external knowledge base.  
2. Combining the retrieved context with the model’s original prompt.  
3. Fine-tuning the model on this retrieval-augmented data.  

This approach ensures the model learns to ground its answers in facts while still benefiting from general reasoning abilities.

---

## Lesson Overview

In this notebook, we will:  
- Introduce **RAFT** and why it’s important for domain-specific LLMs.  
- Generate a synthetic dataset by pairing **prompts** with **retrieved context**.  
- Format the data into instruction-style samples.  
- Validate dataset structure and content quality.  
- Estimate token usage for future fine-tuning.  

---

## Dataset Preparation

The RAFT workflow typically involves:  
- **Knowledge corpus**: A collection of domain documents (e.g., policies, manuals, FAQs).  
- **Query generation**: Creating prompts that a user might ask.  
- **Retrieval step**: Using a retriever (BM25, FAISS, or vector DB) to fetch relevant passages.  
- **Data formatting**: Building `(instruction, input, output)` training triples.  

---

## Data Validation

To ensure dataset quality, we:  
- Check for missing fields (`instruction`, `input`, `output`).  
- Ensure context is relevant to the query.  
- Filter out low-quality or duplicate entries.  

---

## Token Counting & Statistics

Fine-tuning cost and performance depend heavily on token counts.  

In this lesson, we:  
- Use [tiktoken](https://github.com/openai/tiktoken) to estimate tokens.  
- Review average input and output length.  
- Calculate overall dataset size to plan fine-tuning runs.  

---

## Review & Self Study

This lesson showed how to:  
- Build a **retrieval-augmented dataset** for fine-tuning.  
- Ensure data quality with validation and filtering.  
- Prepare training-ready samples in structured format.  

### Further Study
- [RAG vs. Fine-Tuning Explained](https://www.ibm.com/think/topics/rag-vs-fine-tuning)  
- [Hugging Face Retrieval-Augmented Models](https://huggingface.co/docs/transformers/main/en/model_doc/rag)  
- Explore vector DBs like [FAISS](https://faiss.ai/) or [Weaviate](https://weaviate.io/).  

---

## Assignment

**RAFT Dataset Demo** – create a retrieval-augmented dataset.  
- Select a small knowledge base (e.g., a Wikipedia dump, course handbook, or documentation set).  
- Generate at least 5 user queries.  
- Run a retriever to fetch relevant context for each query.  
- Format the data into `(instruction, input, output)` triples.  
- Inspect token usage and dataset size.  
