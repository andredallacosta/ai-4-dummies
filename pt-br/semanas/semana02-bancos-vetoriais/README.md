# Semana 2: Bancos Vetoriais na Prática

## 🎯 Objetivo Geral
Dominar o uso prático de bancos vetoriais para armazenamento e busca semântica eficiente, comparando diferentes soluções e implementando sistemas de busca em produção.

---

## 📅 Cronograma Diário (7 dias)

### **Dia 1: Teoria dos Bancos Vetoriais**
**Tempo:** 30-45 min  
**Objetivo:** Entender conceitos fundamentais e arquiteturas de bancos vetoriais

**Atividades:**
- [ ] 📖 Ler: [What are Vector Databases?](https://www.pinecone.io/learn/vector-database/)
- [ ] 📖 Ler: [Vector Databases Explained](https://weaviate.io/blog/what-is-a-vector-database)
- [ ] 📝 Mapear diferenças: banco vetorial vs banco tradicional
- [ ] 🧠 Listar 5 casos de uso para bancos vetoriais
- [ ] 📝 Comparar arquiteturas: index-based vs graph-based

**Resultado esperado:** Compreensão sólida do que são bancos vetoriais e quando usar

---

### **Dia 2: ChromaDB Setup e Básico**
**Tempo:** 45-60 min  
**Objetivo:** Configurar ChromaDB e realizar primeiras operações

**Atividades:**
- [ ] ⚙️ Instalar ChromaDB: `pip install chromadb`
- [ ] 👨‍💻 Criar `exemplo_01_chromadb_basico.py`: primeira coleção
- [ ] 🧪 Operações básicas:
  - Criar coleção
  - Inserir documentos com embeddings
  - Busca por similaridade
- [ ] 📊 Testar com 10-20 documentos simples
- [ ] 📝 Documentar configurações e comportamentos

**Resultado esperado:** ChromaDB funcionando com operações básicas

---

### **Dia 3: CRUD Completo e Persistência**
**Tempo:** 45-60 min  
**Objetivo:** Implementar todas as operações e persistência de dados

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_02_crud_completo.py`
- [ ] 🔧 Implementar:
  - Create: inserção de documentos
  - Read: busca e filtragem
  - Update: atualização de documentos
  - Delete: remoção de documentos
- [ ] 💾 Configurar persistência local
- [ ] 🧪 Testar com dataset maior (100+ documentos)
- [ ] 📝 Melhores práticas para operações CRUD

**Resultado esperado:** Sistema CRUD completo e persistente

---

### **Dia 4: Otimização e Performance**
**Tempo:** 45-60 min  
**Objetivo:** Otimizar queries e medir performance

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_03_performance.py`
- [ ] 📊 Implementar benchmarks:
  - Tempo de inserção
  - Latência de busca
  - Throughput de queries
- [ ] 🔧 Testar configurações:
  - Diferentes tamanhos de embedding
  - Variados números de documentos
  - Filtros e metadados
- [ ] 📈 Analisar performance vs precisão
- [ ] 📝 Guia de otimização

**Resultado esperado:** Sistema otimizado com métricas de performance

---

### **Dia 5: Comparação de Bancos Vetoriais**
**Tempo:** 45-60 min  
**Objetivo:** Comparar ChromaDB com outras soluções

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_04_comparacao.py`
- [ ] 🧪 Implementar busca com:
  - ChromaDB (já implementado)
  - FAISS (Facebook AI Similarity Search)
  - Qdrant (se possível)
- [ ] 📊 Comparar:
  - Facilidade de uso
  - Performance
  - Recursos disponíveis
  - Escalabilidade
- [ ] 📝 Matriz de comparação detalhada

**Resultado esperado:** Análise comparativa completa de soluções

---

### **Dia 6: Integração com Aplicações**
**Tempo:** 45-60 min  
**Objetivo:** Criar API REST para banco vetorial

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_05_api_rest.py`
- [ ] 🌐 Implementar endpoints FastAPI:
  - POST /documents (inserir)
  - GET /search (buscar)
  - PUT /documents/{id} (atualizar)
  - DELETE /documents/{id} (deletar)
- [ ] 🧪 Testar com Postman ou curl
- [ ] 📊 Adicionar métricas e logging
- [ ] 📝 Documentação da API com OpenAPI

**Resultado esperado:** API REST funcionando para banco vetorial

---

### **Dia 7: Mini-Projeto Final**
**Tempo:** 60-90 min  
**Objetivo:** Sistema de busca semântica completo com interface web

**Atividades:**
- [ ] 👨‍💻 Criar `mini_projeto_busca_semantica/`
- [ ] 🏗️ Implementar sistema completo:
  - Backend FastAPI com ChromaDB
  - Interface web com Streamlit
  - Upload de documentos (PDF, TXT)
  - Busca semântica em tempo real
- [ ] 📊 Features avançadas:
  - Filtros por metadados
  - Histórico de buscas
  - Métricas de relevância
  - Export de resultados
- [ ] 🧪 Testar com dataset real (artigos, documentos)
- [ ] 📝 README com arquitetura e guia de uso
- [ ] 🎉 Demo funcionando end-to-end

**Resultado esperado:** Sistema de busca semântica production-ready

---

## 📚 Recursos de Estudo

### **Leituras Essenciais**
- [ChromaDB Documentation](https://docs.trychroma.com/)
- [Vector Databases Explained](https://www.pinecone.io/learn/vector-database/)
- [FAISS Documentation](https://faiss.ai/index.html)

### **Leituras Complementares**
- [Qdrant Documentation](https://qdrant.tech/documentation/)
- [Weaviate Concepts](https://weaviate.io/developers/weaviate/concepts)
- [Vector Search Algorithms](https://blog.research.google/2020/07/announcing-scann-efficient-vector.html)

### **Vídeos Recomendados**
- [ChromaDB in 5 Minutes](https://www.youtube.com/watch?v=QdDoFfkVkcw)
- [Vector Databases Comparison](https://www.youtube.com/watch?v=klTvEwg3oJ4)

---

## 🛠️ Setup Técnico

### **Dependências**
```bash
# Adicionar ao requirements.txt
chromadb==0.4.18
faiss-cpu==1.7.4
qdrant-client==1.6.9
fastapi==0.104.1
uvicorn==0.24.0
streamlit==1.28.2
sentence-transformers==2.2.2
pandas==2.0.3
numpy==1.24.3
requests==2.31.0
pypdf==3.17.1
python-multipart==0.0.6
```

### **Estrutura de Arquivos**
```
semana02-bancos-vetoriais/
├── README.md                         # Este arquivo
├── experimentos.md                   # Suas anotações
├── exemplos/
│   ├── exemplo_01_chromadb_basico.py
│   ├── exemplo_02_crud_completo.py
│   ├── exemplo_03_performance.py
│   ├── exemplo_04_comparacao.py
│   └── exemplo_05_api_rest.py
└── mini-projeto/
    ├── mini_projeto_busca_semantica/
    │   ├── backend/
    │   │   ├── main.py               # FastAPI app
    │   │   ├── vector_db.py          # ChromaDB operations
    │   │   └── models.py             # Pydantic models
    │   ├── frontend/
    │   │   └── app.py                # Streamlit interface
    │   ├── data/                     # Documentos de teste
    │   └── requirements.txt
    └── README.md
```

---

## ✅ Checklist de Aprendizado

### **Conceitos Teóricos**
- [ ] Entendo diferenças entre bancos vetoriais e tradicionais
- [ ] Conheço principais algoritmos de busca vetorial
- [ ] Sei quando usar cada tipo de banco vetorial
- [ ] Compreendo trade-offs performance vs precisão

### **Habilidades Práticas**
- [ ] Configurei e usei ChromaDB
- [ ] Implementei operações CRUD completas
- [ ] Otimizei performance de queries
- [ ] Comparei diferentes soluções
- [ ] Criei API REST para banco vetorial

### **Projeto Final**
- [ ] Sistema de busca semântica funcionando
- [ ] Interface web intuitiva
- [ ] API documentada
- [ ] Performance otimizada
- [ ] Documentação completa

---

## 📝 Espaço para Anotações

### **Comparação de Soluções**
- **ChromaDB:**
  - Prós:
  - Contras:
  - Melhor para:

- **FAISS:**
  - Prós:
  - Contras:
  - Melhor para:

### **Métricas de Performance**
- Tempo de inserção:
- Latência de busca:
- Precisão dos resultados:
- Uso de memória:

### **Configurações Ótimas**
- Tamanho de embedding:
- Algoritmo de busca:
- Parâmetros de index:

### **Problemas Encontrados**
- (Dificuldades técnicas e soluções)

### **Ideias para Próximos Projetos**
- (Aplicações práticas com bancos vetoriais)