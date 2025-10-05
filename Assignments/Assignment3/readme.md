### creating readme
 
### Simplified Agentic RAG System with Gemini & LangGraph

Retrieval-Augmented Generation (RAG) combines a knowledge base (KB)
with a Large Language Model (LLM) so answers are grounded in factual content.
An agentic RAG adds a self-review loop: the model critiques its own answer,
checks against the KB, and refines if needed.
In this assignment, you will build a lightweight agentic RAG pipeline using:
• Gemini on Google Cloud (Vertex AI) as the LLM
• LangGraph to wire the workflow
2. Problem Statement
“Build a simplified Agentic RAG system with Gemini +
LangGraph that retrieves up to 5 KB snippets, generates an
initial answer, critiques it, and when necessary refines the
answer by pulling one more snippet, returning a citationbacked response.”
Dataset: self_critique_loop_dataset.json
