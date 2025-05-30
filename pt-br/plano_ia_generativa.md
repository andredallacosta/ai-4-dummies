# Plano de Estudo Avançado em IA Generativa, RAG, Agentes e Ferramentas Modernas

**Duração sugerida:** 9 semanas  
**Tempo diário:** 30-60 minutos  
**Foco:** Prática, ferramentas do mercado, projetos reais

---

## Semana 1: Fundamentos Práticos de LLMs e Embeddings
- Revisão rápida: O que são LLMs, embeddings, aplicações modernas
- Gerar embeddings com HuggingFace ou OpenAI
- Leitura:
  - [Embeddings — OpenAI](https://platform.openai.com/docs/guides/embeddings)
  - [Sentence Transformers](https://www.sbert.net/)
- Prática:
  - Gerar embeddings de textos próprios e comparar similaridade

---

## Semana 2: Bancos Vetoriais na Prática
- O que são bancos vetoriais e para que servem
- Principais opções: ChromaDB, Pinecone, Weaviate, Qdrant
- Leitura:
  - [ChromaDB Docs](https://docs.trychroma.com/)
  - [Pinecone Quickstart](https://docs.pinecone.io/docs/quickstart)
- Prática:
  - Indexar e buscar embeddings em um banco vetorial local (ChromaDB ou FAISS)
  - Mini-projeto: busca semântica de textos pessoais

---

## Semana 3: Retrieval-Augmented Generation (RAG)
- Conceito e arquitetura de RAG
- Frameworks: LlamaIndex, LangChain, Haystack
- Leitura:
  - [RAG com LlamaIndex](https://docs.llamaindex.ai/en/stable/getting_started/concepts.html)
  - [RAG com LangChain](https://python.langchain.com/docs/tutorials/rag/)
- Prática:
  - Construir um Q&A simples com RAG usando LlamaIndex ou LangChain

---

## Semana 4: Model Context Protocol (MCP) e Interoperabilidade
- O que é MCP e por que é importante para IA generativa e agentes
- Estrutura do protocolo: contexto, histórico, instruções, resultados
- Principais implementações e frameworks que suportam MCP
- Como usar MCP para integrar diferentes agentes, LLMs e ferramentas
- Leitura:
  - [Model Context Protocol - GitHub](https://github.com/modelcontextprotocol/modelcontextprotocol)
  - [MCP e interoperabilidade em agentes](https://www.anthropic.com/news/model-context-protocol)
- Prática:
  - Integrar dois agentes ou LLMs usando MCP
  - Trocar contexto entre diferentes frameworks (ex: LangChain + LlamaIndex)

---

## Semana 5: Memória, Contexto e Persistência (MCP-Memória)
- Conceito de MCP-Memória e importância para agentes/LLMs
- Tipos de memória: curto e longo prazo
- Ferramentas: LangChain Memory, LlamaIndex Storage, bancos vetoriais
- Persistência de histórico
- Leitura:
  - [LangChain Memory](https://python.langchain.com/api_reference/langchain/memory.html)
  - [LlamaIndex Storage](https://docs.llamaindex.ai/en/stable/module_guides/storing/index.html)
  - [RAG e memória de longo prazo](https://medium.com/aingineer/a-complete-guide-to-implementing-memory-augmented-rag-c3582a8dc74f)
- Prática:
  - Implementar um chatbot com memória de conversação (LangChain ou LlamaIndex)
  - Persistir histórico de interações em um banco vetorial ou arquivo
  - Recuperar contexto de sessões anteriores

---

## Semana 6: Fine Tuning e LoRA
- Fine tuning vs. Prompt Engineering
- LoRA e quantização
- Leitura:
  - [LoRA Paper](https://arxiv.org/abs/2106.09685)
  - [HuggingFace PEFT/LoRA](https://github.com/huggingface/peft)
- Prática:
  - Fine tuning ou LoRA em um modelo pequeno (ex: Alpaca, Llama 2 7B)
  - Testar quantização com bitsandbytes

---

## Semana 7: Agentes de IA e Orquestração
- O que são agentes, tipos e aplicações
- Frameworks: LangChain Agents, CrewAI, AutoGen
- Leitura:
  - [LangChain Agents](https://python.langchain.com/docs/how_to/#agents)
  - [CrewAI](https://docs.crewai.com/)
- Prática:
  - Criar um agente simples para automação de tarefas (ex: busca + sumarização)

---

## Semana 8: Orquestração Avançada e Multi-Agentes
- Orquestração de múltiplos agentes
- Workflows, pipelines e colaboração
- Leitura:
  - [Multi-Agent](https://blog.langchain.dev/langgraph-multi-agent-workflows/)
  - [AutoGen](https://microsoft.github.io/autogen/)
- Prática:
  - Orquestrar dois agentes para resolver um problema em conjunto

---

## Semana 9: Deploy, Observabilidade e Avaliação
- Deploy de modelos e aplicações (FastAPI, TGI, vLLM)
- Monitoramento e avaliação (PromptLayer, LangSmith, Ragas)
- Leitura:
  - [Text Generation Inference](https://github.com/huggingface/text-generation-inference)
  - [LangSmith](https://smith.langchain.com/)
- Prática:
  - Deploy de um Q&A RAG como API
  - Avaliar respostas e ajustar prompts/modelo

---

## Semana 10: Tópicos Avançados e Multi-modalidade
- Multi-modalidade (texto, imagem, áudio)
- Segurança, alinhamento e guardrails
- Leitura:
  - [LLaVA (Vision+Language)](https://llava-vl.github.io/)
  - [Guardrails AI](https://github.com/guardrails-ai/guardrails)
- Prática:
  - Testar um modelo multi-modal (ex: LLaVA, CLIP)
  - Implementar um guardrail simples para filtrar respostas

---

## Dicas Gerais
- Documente tudo: Use um repositório para anotar aprendizados e projetos.
- Participe de comunidades: Discords, Slack, GitHub Discussions de LangChain, LlamaIndex, etc.
- Compartilhe projetos: No GitHub, LinkedIn, etc.

---

**Como usar:**
- Traga a semana/tópico que deseja detalhar e peça exemplos, recursos e exercícios práticos.
- Exemplo: "Quero detalhar a Semana 2 do meu plano de IA generativa." 