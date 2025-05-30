# Semana 5: Memória, Contexto e Persistência

## 🎯 Objetivo Geral
Dominar conceitos e implementação de sistemas de memória para LLMs e agentes, incluindo memória de curto e longo prazo, persistência de contexto e técnicas avançadas de gerenciamento de histórico.

---

## 📅 Cronograma Diário (7 dias)

### **Dia 1: Teoria da Memória em IA**
**Tempo:** 30-45 min  
**Objetivo:** Entender tipos de memória e sua importância para agentes de IA

**Atividades:**
- [ ] 📖 Ler: [Memory in AI Systems](https://python.langchain.com/api_reference/langchain/memory.html)
- [ ] 📖 Ler: [Short vs Long Term Memory](https://arxiv.org/abs/2307.08621)
- [ ] 📝 Resumir diferenças: Working Memory vs Long-term Memory
- [ ] 🧠 Listar 5 cenários onde memória persistente é crucial
- [ ] 📝 Mapear tipos de memória: Episódica, Semântica, Procedural

**Resultado esperado:** Base teórica sólida sobre memória em sistemas de IA

---

### **Dia 2: Memória no LangChain**
**Tempo:** 45-60 min  
**Objetivo:** Implementar diferentes tipos de memória com LangChain

**Atividades:**
- [ ] 📖 Ler: [LangChain Memory Documentation](https://python.langchain.com/api_reference/langchain/memory.html)
- [ ] 👨‍💻 Criar `exemplo_01_memory_types.py`
- [ ] 🧪 Testar diferentes tipos:
  - ConversationBufferMemory
  - ConversationSummaryMemory
  - ConversationBufferWindowMemory
  - VectorStoreRetrieverMemory
- [ ] 📊 Comparar comportamento e uso de memória
- [ ] 📝 Documentar trade-offs de cada tipo

**Resultado esperado:** Domínio prático dos tipos de memória do LangChain

---

### **Dia 3: Persistência com Bancos Vetoriais**
**Tempo:** 45-60 min  
**Objetivo:** Implementar memória de longo prazo usando bancos vetoriais

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_02_vector_memory.py`
- [ ] 🏗️ Setup ChromaDB para persistir conversas
- [ ] 🧪 Implementar:
  - Armazenamento de turnos de conversação
  - Busca semântica no histórico
  - Filtragem por data/sessão
- [ ] 📊 Testar retrieval de contexto relevante
- [ ] 📝 Documentar estratégias de indexação de conversas

**Resultado esperado:** Sistema de memória persistente baseado em similaridade

---

### **Dia 4: Memória Hierárquica**
**Tempo:** 45-60 min  
**Objetivo:** Implementar sistema de memória com múltiplas camadas

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_03_hierarchical_memory.py`
- [ ] 🏗️ Arquitetura de 3 camadas:
  - Buffer imediato (últimas N mensagens)
  - Memória de sessão (resumo da conversa atual)
  - Memória de longo prazo (banco vetorial)
- [ ] 🧪 Implementar algoritmo de consolidação
- [ ] 📊 Testar com conversas longas (100+ turnos)
- [ ] 📝 Analisar eficiência e qualidade do contexto recuperado

**Resultado esperado:** Sistema de memória multi-camada otimizado

---

### **Dia 5: Memória Personalizada e Profiles**
**Tempo:** 45-60 min  
**Objetivo:** Criar sistema de perfis de usuário e memória personalizada

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_04_user_profiles.py`
- [ ] 🏗️ Implementar:
  - Extração automática de preferências
  - Armazenamento de informações pessoais
  - Atualização incremental de perfis
- [ ] 🧪 Testar com múltiplos usuários
- [ ] 📊 Validar persistência entre sessões
- [ ] 📝 Documentar estratégias de privacy e segurança

**Resultado esperado:** Sistema de perfis personalizados persistentes

---

### **Dia 6: Memória com LlamaIndex**
**Tempo:** 45-60 min  
**Objetivo:** Comparar abordagens de memória entre frameworks

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_05_llamaindex_memory.py`
- [ ] 🔄 Implementar memória usando:
  - ChatMemoryBuffer
  - VectorMemory
  - SimpleDocumentStore
- [ ] 📊 Comparar com implementações LangChain
- [ ] 🧪 Testar integração com índices LlamaIndex
- [ ] 📝 Análise comparativa: quando usar cada framework

**Resultado esperado:** Expertise em memória com múltiplos frameworks

---

### **Dia 7: Mini-Projeto Final**
**Tempo:** 60-90 min  
**Objetivo:** Chatbot avançado com memória persistente completa

**Atividades:**
- [ ] 👨‍💻 Criar `mini_projeto_chatbot_memoria/`
- [ ] 🏗️ Features implementadas:
  - Memória multi-camada (buffer + sessão + longo prazo)
  - Perfis de usuário personalizados
  - Busca no histórico de conversas
  - Interface web com Streamlit
- [ ] 🧪 Funcionalidades:
  - "Lembra quando falamos sobre X?"
  - "Meu perfil mostra que eu gosto de..."
  - Contexto automático baseado em histórico
- [ ] 📊 Dashboard de memória: estatísticas e visualizações
- [ ] 📝 README com arquitetura e guia de uso
- [ ] 🎉 Demo completa com múltiplas sessões

**Resultado esperado:** Chatbot production-ready com memória avançada

---

## 📚 Recursos de Estudo

### **Leituras Essenciais**
- [LangChain Memory](https://python.langchain.com/api_reference/langchain/memory.html)
- [LlamaIndex Storage](https://docs.llamaindex.ai/en/stable/module_guides/storing/index.html)
- [Vector Databases for Memory](https://python.langchain.com/api_reference/langchain/memory.html)

### **Leituras Complementares**
- [Memory-Augmented Neural Networks](https://arxiv.org/abs/1603.03129)
- [Conversation Patterns](https://rasa.com/docs/learn/concepts/conversation-patterns/)
- [RAG vs Memory Systems](https://python.langchain.com/docs/tutorials/rag/)

### **Papers Relevantes**
- [MemGPT: Towards LLMs as Operating Systems](https://arxiv.org/abs/2310.08560)
- [Longformer: The Long-Document Transformer](https://arxiv.org/abs/2004.05150)

---

## 🛠️ Setup Técnico

### **Dependências**
```bash
# Adicionar ao requirements.txt
langchain==0.0.340
llama-index==0.9.13
chromadb==0.4.18
streamlit==1.28.2
sqlite3  # Built-in
redis==5.0.1
sqlalchemy==2.0.23
python-dotenv==1.0.0
plotly==5.17.0
pandas==2.0.3
```

### **Estrutura de Arquivos**
```
semana05-memoria/
├── notas.md                          # Este arquivo
├── experimentos.md                   # Suas anotações
├── exemplos/
│   ├── exemplo_01_memory_types.py
│   ├── exemplo_02_vector_memory.py
│   ├── exemplo_03_hierarchical_memory.py
│   ├── exemplo_04_user_profiles.py
│   └── exemplo_05_llamaindex_memory.py
└── mini-projeto/
    ├── mini_projeto_chatbot_memoria/
    │   ├── app.py                    # Interface Streamlit
    │   ├── memory_manager.py         # Sistema de memória
    │   ├── user_profiles.py          # Gerenciamento de perfis
    │   ├── chat_engine.py           # Engine principal
    │   ├── database/                # Persistência
    │   └── requirements.txt
    └── README.md
```

---

## ✅ Checklist de Aprendizado

### **Conceitos Teóricos**
- [ ] Entendo diferenças entre tipos de memória
- [ ] Sei quando usar cada estratégia de persistência
- [ ] Compreendo trade-offs memória vs performance
- [ ] Conheço limitações de cada abordagem

### **Habilidades Práticas**
- [ ] Implementei todos os tipos de memória LangChain
- [ ] Criei sistema de memória com bancos vetoriais
- [ ] Construí memória hierárquica multi-camada
- [ ] Implementei perfis de usuário personalizados
- [ ] Comparei LangChain vs LlamaIndex para memória

### **Projeto Final**
- [ ] Chatbot com memória persistente completa
- [ ] Interface web funcional
- [ ] Sistema de perfis de usuário
- [ ] Dashboard de analytics de memória
- [ ] Documentação completa

---

## 📝 Espaço para Anotações

### **Comparação de Tipos de Memória**
- **ConversationBufferMemory:**
  - Prós:
  - Contras:
  - Melhor para:

- **VectorStoreRetrieverMemory:**
  - Prós:
  - Contras:
  - Melhor para:

### **Estratégias de Consolidação**
- Quando consolidar:
- Como consolidar:
- Métricas para decidir:

### **Performance Observada**
- Latência de retrieval:
- Uso de memória:
- Qualidade do contexto:

### **Problemas Enfrentados**
- (Dificuldades técnicas e soluções encontradas)

### **Padrões que Funcionaram**
- (Arquitecturas e implementações bem-sucedidas)

### **Ideias para Melhorias**
- (Próximos passos e otimizações possíveis) 