# Advanced Study Plan for Generative AI, RAG, Agents and Modern Tools

**Suggested duration:** 9 weeks  
**Daily time:** 30-60 minutes  
**Focus:** Practice, market tools, real projects

---

## Week 1: Practical Fundamentals of LLMs and Embeddings
- Quick review: What are LLMs, embeddings, modern applications
- Generate embeddings with HuggingFace or OpenAI
- Reading:
  - [Embeddings — OpenAI](https://platform.openai.com/docs/guides/embeddings)
  - [Sentence Transformers](https://www.sbert.net/)
- Practice:
  - Generate embeddings from your own texts and compare similarity

---

## Week 2: Vector Databases in Practice
- What are vector databases and what they're used for
- Main options: ChromaDB, Pinecone, Weaviate, Qdrant
- Reading:
  - [ChromaDB Docs](https://docs.trychroma.com/)
  - [Pinecone Quickstart](https://docs.pinecone.io/docs/quickstart)
- Practice:
  - Index and search embeddings in a local vector database (ChromaDB or FAISS)
  - Mini-project: semantic search of personal texts

---

## Week 3: Retrieval-Augmented Generation (RAG)
- RAG concept and architecture
- Frameworks: LlamaIndex, LangChain, Haystack
- Reading:
  - [RAG with LlamaIndex](https://docs.llamaindex.ai/en/stable/getting_started/concepts.html)
  - [RAG with LangChain](https://python.langchain.com/docs/use_cases/question_answering/)
- Practice:
  - Build a simple Q&A with RAG using LlamaIndex or LangChain

---

## Week 4: Model Context Protocol (MCP) and Interoperability
- What is MCP and why it's important for generative AI and agents
- Protocol structure: context, history, instructions, results
- Main implementations and frameworks that support MCP
- How to use MCP to integrate different agents, LLMs and tools
- Reading:
  - [Model Context Protocol - GitHub](https://github.com/modelcontext/protocol)
  - [MCP and interoperability in agents](https://blog.langchain.dev/model-context-protocol/)
- Practice:
  - Integrate two agents or LLMs using MCP
  - Exchange context between different frameworks (e.g.: LangChain + LlamaIndex)

---

## Week 5: Memory, Context and Persistence (MCP-Memory)
- MCP-Memory concept and importance for agents/LLMs
- Types of memory: short and long term
- Tools: LangChain Memory, LlamaIndex Storage, vector databases
- History persistence
- Reading:
  - [LangChain Memory](https://python.langchain.com/docs/modules/memory/)
  - [LlamaIndex Storage](https://docs.llamaindex.ai/en/stable/module_guides/storing/index.html)
  - [RAG and long-term memory](https://blog.langchain.dev/long-term-memory/)
- Practice:
  - Implement a chatbot with conversation memory (LangChain or LlamaIndex)
  - Persist interaction history in a vector database or file
  - Retrieve context from previous sessions

---

## Week 6: Fine Tuning and LoRA
- Fine tuning vs. Prompt Engineering
- LoRA and quantization
- Reading:
  - [LoRA Paper](https://arxiv.org/abs/2106.09685)
  - [HuggingFace PEFT/LoRA](https://github.com/huggingface/peft)
- Practice:
  - Fine tuning or LoRA on a small model (e.g.: Alpaca, Llama 2 7B)
  - Test quantization with bitsandbytes

---

## Week 7: AI Agents and Orchestration
- What are agents, types and applications
- Frameworks: LangChain Agents, CrewAI, AutoGen
- Reading:
  - [LangChain Agents](https://python.langchain.com/docs/modules/agents/)
  - [CrewAI](https://docs.crewai.com/)
- Practice:
  - Create a simple agent for task automation (e.g.: search + summarization)

---

## Week 8: Advanced Orchestration and Multi-Agents
- Multiple agent orchestration
- Workflows, pipelines and collaboration
- Reading:
  - [LangChain Multi-Agent](https://python.langchain.com/docs/modules/agents/multi_agent)
  - [AutoGen](https://microsoft.github.io/autogen/)
- Practice:
  - Orchestrate two agents to solve a problem together

---

## Week 9: Deploy, Observability and Evaluation
- Model and application deployment (FastAPI, TGI, vLLM)
- Monitoring and evaluation (PromptLayer, LangSmith, Ragas)
- Reading:
  - [Text Generation Inference](https://github.com/huggingface/text-generation-inference)
  - [LangSmith](https://smith.langchain.com/)
- Practice:
  - Deploy a RAG Q&A as API
  - Evaluate responses and adjust prompts/model

---

## Week 10: Advanced Topics and Multi-modality
- Multi-modality (text, image, audio)
- Security, alignment and guardrails
- Reading:
  - [LLaVA (Vision+Language)](https://llava-vl.github.io/)
  - [Guardrails AI](https://shreyar.github.io/guardrails/)
- Practice:
  - Test a multi-modal model (e.g.: LLaVA, CLIP)
  - Implement a simple guardrail to filter responses

---

## General Tips
- Document everything: Use a repository to note learnings and projects.
- Join communities: Discords, Slack, GitHub Discussions of LangChain, LlamaIndex, etc.
- Share projects: On GitHub, LinkedIn, etc.

---

**How to use:**
- Bring the week/topic you want to detail and ask for examples, resources and practical exercises.
- Example: "I want to detail Week 2 of my generative AI plan." 