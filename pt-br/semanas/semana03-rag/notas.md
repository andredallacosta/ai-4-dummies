# Semana 3: Retrieval-Augmented Generation (RAG)

## 🎯 Objetivo Geral
Dominar o conceito e implementação prática de RAG (Retrieval-Augmented Generation), combinando busca semântica com geração de texto para criar sistemas de Q&A inteligentes.

---

## 📅 Cronograma Diário (7 dias)

### **Dia 1: Teoria e Arquitetura RAG**
**Tempo:** 30-45 min  
**Objetivo:** Entender completamente o conceito de RAG e sua arquitetura

**Atividades:**
- [ ] 📖 Ler: [What is RAG?](https://blogs.nvidia.com/blog/2023/11/13/what-is-retrieval-augmented-generation/)
- [ ] 📖 Ler: [RAG vs Fine Tuning](https://www.pinecone.io/learn/retrieval-augmented-generation/)
- [ ] 📝 Desenhar diagrama da arquitetura RAG (Retrieval → Augmentation → Generation)
- [ ] 🧠 Listar 5 casos de uso onde RAG é melhor que fine-tuning
- [ ] 📝 Resumir vantagens e limitações do RAG

**Resultado esperado:** Compreensão sólida do que é RAG e quando usar

---

### **Dia 2: LangChain Fundamentals**
**Tempo:** 45-60 min  
**Objetivo:** Setup e primeiros passos com LangChain para RAG

**Atividades:**
- [ ] 📖 Ler: [LangChain RAG Tutorial](https://python.langchain.com/docs/use_cases/question_answering/)
- [ ] ⚙️ Instalar dependências: langchain, openai, chromadb
- [ ] 👨‍💻 Criar `exemplo_01_langchain_basico.py`: loader + splitter + embeddings
- [ ] 🧪 Testar com documento de texto simples (PDF ou TXT)
- [ ] 📝 Documentar cada componente: DocumentLoader, TextSplitter, VectorStore

**Resultado esperado:** Pipeline básico de ingesting de documentos funcionando

---

### **Dia 3: LlamaIndex Fundamentals**
**Tempo:** 45-60 min  
**Objetivo:** Comparar abordagem do LlamaIndex vs LangChain

**Atividades:**
- [ ] 📖 Ler: [LlamaIndex Quickstart](https://docs.llamaindex.ai/en/stable/getting_started/starter_example.html)
- [ ] ⚙️ Instalar llama-index
- [ ] 👨‍💻 Criar `exemplo_02_llamaindex_basico.py`: SimpleDirectoryReader + VectorStoreIndex
- [ ] 🧪 Usar mesmo documento do dia anterior
- [ ] 📊 Comparar: facilidade de uso, velocidade, qualidade das respostas
- [ ] 📝 Documentar diferenças entre LangChain e LlamaIndex

**Resultado esperado:** Domínio de dois principais frameworks para RAG

---

### **Dia 4: Chunking Strategies**
**Tempo:** 45-60 min  
**Objetivo:** Otimizar estratégias de divisão de texto para melhor retrieval

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_03_chunking_strategies.py`
- [ ] 🧪 Testar diferentes abordagens:
  - Character splitting (tamanho fixo)
  - Recursive character splitting
  - Semantic chunking
  - Document-aware splitting
- [ ] 📊 Comparar qualidade das respostas para cada método
- [ ] 🔍 Analisar: qual chunking funciona melhor para que tipo de documento?
- [ ] 📝 Documentar melhores práticas de chunking

**Resultado esperado:** Expertise em otimização de chunking para diferentes cenários

---

### **Dia 5: Prompt Engineering para RAG**
**Tempo:** 45-60 min  
**Objetivo:** Melhorar qualidade das respostas através de prompt engineering

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_04_prompt_engineering.py`
- [ ] 🧪 Testar diferentes templates de prompt:
  - Basic: "Answer based on context: {context}\nQuestion: {question}"
  - Detailed: Instruções específicas sobre como responder
  - Chain-of-thought: Pedir para explicar raciocínio
  - Few-shot: Incluir exemplos
- [ ] 📊 Avaliar qualidade das respostas para cada template
- [ ] 🔍 Identificar quando cada tipo de prompt funciona melhor
- [ ] 📝 Criar biblioteca de prompts reutilizáveis

**Resultado esperado:** Biblioteca de prompts otimizados para diferentes casos de uso

---

### **Dia 6: Avaliação e Métricas**
**Tempo:** 45-60 min  
**Objetivo:** Implementar métricas para avaliar qualidade do sistema RAG

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_05_avaliacao.py`
- [ ] 📊 Implementar métricas:
  - Relevância dos documentos recuperados
  - Qualidade das respostas (BLEU, ROUGE se possível)
  - Tempo de resposta
- [ ] 🧪 Criar dataset de test com perguntas e respostas esperadas
- [ ] 📈 Comparar performance de diferentes configurações
- [ ] 📝 Dashboard simples para visualizar métricas

**Resultado esperado:** Sistema de avaliação automatizada do RAG

---

### **Dia 7: Mini-Projeto Final**
**Tempo:** 60-90 min  
**Objetivo:** Q&A system completo sobre documentos próprios

**Atividades:**
- [ ] 👨‍💻 Criar `mini_projeto_qa_pessoal.py`
- [ ] 📚 Dataset: Documentos pessoais (PDFs, artigos salvos, notas)
- [ ] 🏗️ Pipeline completo: ingestão → chunking → embedding → retrieval → geração
- [ ] 💻 Interface: Streamlit ou gradio para interação
- [ ] 🧪 Testar com perguntas complexas sobre seus documentos
- [ ] 📊 Incluir métricas de avaliação em tempo real
- [ ] 📝 README detalhado com arquitetura e resultados
- [ ] 🎉 Demo funcionando + análise de limitações

**Resultado esperado:** Sistema RAG completo e funcional para uso pessoal

---

## 📚 Recursos de Estudo

### **Leituras Essenciais**
- [RAG com LlamaIndex](https://docs.llamaindex.ai/en/stable/getting_started/concepts.html)
- [RAG com LangChain](https://python.langchain.com/docs/use_cases/question_answering/)
- [Chunking Strategies](https://www.pinecone.io/learn/chunking-strategies/)

### **Leituras Complementares**
- [Advanced RAG Techniques](https://blog.langchain.dev/semi-structured-multi-modal-rag/)
- [RAG vs Fine-tuning](https://www.anyscale.com/blog/a-comprehensive-guide-for-building-rag-based-llm-applications-part-1)
- [Evaluation of RAG Systems](https://blog.langchain.dev/evaluating-rag-pipelines-with-ragas-langsmith/)

### **Vídeos Recomendados**
- [LangChain RAG from Scratch](https://www.youtube.com/watch?v=LhnCsygAvzY)
- [LlamaIndex in 5 Minutes](https://www.youtube.com/watch?v=hA1JPOy9KCc)

---

## 🛠️ Setup Técnico

### **Dependências**
```bash
# Adicionar ao requirements.txt
langchain==0.0.340
llama-index==0.9.13
openai==1.3.5
chromadb==0.4.18
tiktoken==0.5.1
pypdf==3.17.1
streamlit==1.28.2
gradio==4.7.1
sentence-transformers==2.2.2
faiss-cpu==1.7.4
```

### **Estrutura de Arquivos**
```
semana03-rag/
├── notas.md                          # Este arquivo
├── experimentos.md                   # Suas anotações
├── exemplos/
│   ├── exemplo_01_langchain_basico.py
│   ├── exemplo_02_llamaindex_basico.py
│   ├── exemplo_03_chunking_strategies.py
│   ├── exemplo_04_prompt_engineering.py
│   └── exemplo_05_avaliacao.py
└── mini-projeto/
    ├── mini_projeto_qa_pessoal.py
    ├── interface_streamlit.py
    ├── documentos/                   # Seus documentos de teste
    ├── prompts_library.py
    └── README.md
```

---

## ✅ Checklist de Aprendizado

### **Conceitos Teóricos**
- [ ] Consigo explicar RAG vs fine-tuning em 3 minutos
- [ ] Entendo os componentes: Retrieval, Augmentation, Generation
- [ ] Sei quando usar LangChain vs LlamaIndex
- [ ] Conheço diferentes estratégias de chunking

### **Habilidades Práticas**
- [ ] Implementei RAG com LangChain
- [ ] Implementei RAG com LlamaIndex
- [ ] Testei diferentes estratégias de chunking
- [ ] Criei prompts otimizados para RAG
- [ ] Implementei sistema de avaliação

### **Projeto Final**
- [ ] Q&A system funcionando com documentos próprios
- [ ] Interface web para interação
- [ ] Métricas de avaliação implementadas
- [ ] Documentação completa

---

## 📝 Espaço para Anotações

### **Comparação LangChain vs LlamaIndex**
- **LangChain:**
  - Prós:
  - Contras:
- **LlamaIndex:**
  - Prós:
  - Contras:

### **Melhores Estratégias de Chunking**
- Para documentos técnicos:
- Para narrativas/livros:
- Para artigos acadêmicos:

### **Prompts que Funcionaram Bem**
- (Cole aqui os prompts que deram melhores resultados)

### **Limitações Identificadas**
- (O que não funcionou bem? Que problemas encontrou?)

### **Ideias para Próximos Projetos**
- (Inspirações para projetos mais avançados com RAG) 