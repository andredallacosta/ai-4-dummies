# Semana 1: Fundamentos Práticos de LLMs e Embeddings

## 🎯 Objetivo Geral
Compreender na teoria e prática o que são LLMs e embeddings, como gerá-los e usá-los para tarefas reais de similaridade semântica.

---

## 📅 Cronograma Diário (7 dias)

### **Dia 1: Teoria dos LLMs**
**Tempo:** 30-45 min  
**Objetivo:** Entender o panorama atual dos LLMs

**Atividades:**
- [ ] 📖 Ler: [What are Large Language Models (LLMs)?](https://aws.amazon.com/what-is/large-language-model/)
- [ ] 📖 Ler: [The Illustrated Transformer](http://jalammar.github.io/illustrated-transformer/) (primeiros 50%)
- [ ] 📝 Resumir em 3 parágrafos: O que são LLMs e por que são importantes
- [ ] 🧠 Listar 5 aplicações práticas de LLMs que você conhece

**Resultado esperado:** Vocabulário básico sobre LLMs e transformers

---

### **Dia 2: Teoria dos Embeddings**
**Tempo:** 30-45 min  
**Objetivo:** Entender o conceito de embeddings e suas aplicações

**Atividades:**
- [ ] 📖 Ler: [What are embeddings?](https://platform.openai.com/docs/guides/embeddings/what-are-embeddings)
- [ ] 📖 Ler: [Word2Vec Explained](https://towardsdatascience.com/word2vec-explained-49c52b4ccb71)
- [ ] 📝 Criar um mapa mental: tipos de embeddings (palavra, frase, documento)
- [ ] 🧠 Pensar em 3 casos de uso para embeddings no seu contexto profissional/pessoal

**Resultado esperado:** Compreensão clara de como embeddings capturam significado

---

### **Dia 3: Setup e Primeiro Código**
**Tempo:** 45-60 min  
**Objetivo:** Configurar ambiente e gerar primeiros embeddings

**Atividades:**
- [ ] ⚙️ Setup do ambiente Python (requirements.txt)
- [ ] 👨‍💻 Criar `exemplo_01_basico.py`: Gerar embeddings com Sentence Transformers
- [ ] 🧪 Testar com 3-5 frases simples
- [ ] 📊 Printar dimensões e primeiros valores dos embeddings
- [ ] 📝 Documentar observações no arquivo `experimentos.md`

**Resultado esperado:** Ambiente funcionando + primeiros embeddings gerados

---

### **Dia 4: Comparação de Similaridade**
**Tempo:** 45-60 min  
**Objetivo:** Calcular e interpretar similaridade semântica

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_02_similaridade.py`: calcular cosine similarity
- [ ] 🧪 Testar com pares de frases: similares vs diferentes
- [ ] 📊 Criar uma tabela de resultados (frase1, frase2, similaridade)
- [ ] 🔍 Investigar: Por que algumas frases têm alta similaridade?
- [ ] 📝 Documentar insights sobre limitações e surpresas

**Resultado esperado:** Compreensão prática de como medir similaridade semântica

---

### **Dia 5: Comparação de Modelos**
**Tempo:** 45-60 min  
**Objetivo:** Testar diferentes modelos de embeddings

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_03_comparacao_modelos.py`
- [ ] 🧪 Testar pelo menos 3 modelos: 
  - `all-MiniLM-L6-v2` (rápido)
  - `all-mpnet-base-v2` (melhor qualidade)
  - `distilbert-base-multilingual-cased` (multilingual)
- [ ] 📊 Comparar resultados de similaridade para o mesmo conjunto de frases
- [ ] ⏱️ Medir tempo de processamento de cada modelo
- [ ] 📝 Análise: trade-off entre velocidade e qualidade

**Resultado esperado:** Conhecimento prático das diferenças entre modelos

---

### **Dia 6: Visualização**
**Tempo:** 45-60 min  
**Objetivo:** Visualizar embeddings em 2D para intuição geométrica

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_04_visualizacao.py`
- [ ] 📊 Usar t-SNE ou UMAP para reduzir dimensionalidade
- [ ] 🎨 Plotar embeddings com matplotlib/plotly
- [ ] 🏷️ Colorir pontos por categorias (se aplicável)
- [ ] 🔍 Interpretar: clusters fazem sentido semântico?
- [ ] 📝 Capturar screenshots dos plots

**Resultado esperado:** Intuição visual de como embeddings organizam informação semântica

---

### **Dia 7: Mini-Projeto Final**
**Tempo:** 60-90 min  
**Objetivo:** Consolidar aprendizado em projeto prático

**Atividades:**
- [ ] 👨‍💻 Criar `mini_projeto_busca_semantica.py`
- [ ] 📚 Dataset: 20-30 frases sobre temas variados
- [ ] 🔍 Implementar busca semântica: dado um query, retornar top-3 mais similares
- [ ] 📊 Interface simples: input do usuário → resultados rankeados
- [ ] 🧪 Testar com queries interessantes
- [ ] 📝 README do mini-projeto com exemplos e resultados
- [ ] 🎉 Celebrar! Documentar aprendizados gerais da semana

**Resultado esperado:** Aplicação funcional de busca semântica

---

## 📚 Recursos de Estudo

### **Leituras Essenciais**
- [Embeddings — OpenAI](https://platform.openai.com/docs/guides/embeddings)
- [Sentence Transformers Documentation](https://www.sbert.net/)
- [The Illustrated Transformer](http://jalammar.github.io/illustrated-transformer/)

### **Leituras Complementares**
- [HuggingFace Transformers Course](https://huggingface.co/learn/nlp-course/chapter1/1)
- [OpenAI Cookbook: Embeddings](https://github.com/openai/openai-cookbook/blob/main/examples/Getting_embeddings.ipynb)
- [Awesome Embeddings Papers](https://github.com/Separius/awesome-sentence-embedding)

### **Comunidades**
- [HuggingFace Discord](https://discord.gg/JfAtkvEtRb)
- [r/MachineLearning](https://reddit.com/r/MachineLearning)
- [OpenAI Community](https://community.openai.com/)

---

## 🛠️ Setup Técnico

### **Dependências**
```bash
# Adicionar ao requirements.txt
sentence-transformers==2.2.2
numpy==1.24.3
matplotlib==3.7.1
scikit-learn==1.3.0
umap-learn==0.5.3
plotly==5.15.0
pandas==2.0.3
```

### **Estrutura de Arquivos**
```
semana01-llms-embeddings/
├── notas.md                           # Este arquivo
├── experimentos.md                    # Suas anotações
├── exemplos/
│   ├── exemplo_01_basico.py
│   ├── exemplo_02_similaridade.py
│   ├── exemplo_03_comparacao_modelos.py
│   └── exemplo_04_visualizacao.py
└── mini-projeto/
    ├── mini_projeto_busca_semantica.py
    ├── dataset_exemplo.txt
    └── README.md
```

---

## ✅ Checklist de Aprendizado

### **Conceitos Teóricos**
- [ ] Consigo explicar o que são LLMs em 2 minutos
- [ ] Entendo a diferença entre embeddings de palavra vs frase vs documento
- [ ] Sei explicar cosine similarity e quando usar
- [ ] Conheço pelo menos 3 aplicações práticas de embeddings

### **Habilidades Práticas**
- [ ] Consigo gerar embeddings com Sentence Transformers
- [ ] Sei calcular similaridade entre textos
- [ ] Testei pelo menos 3 modelos diferentes
- [ ] Criei visualização 2D de embeddings
- [ ] Implementei busca semântica básica

### **Projeto Final**
- [ ] Mini-projeto funciona corretamente
- [ ] Documentei código e resultados
- [ ] Identifiquei limitações e próximos passos

---

## 📝 Espaço para Anotações

### **Dúvidas**
- (Anote aqui suas dúvidas para pesquisar depois)

### **Insights**
- (O que mais te surpreendeu? O que funcionou melhor/pior que esperado?)

### **Ideias de Projetos**
- (Inspirações para projetos futuros usando embeddings)

### **Links Extras**
- (Recursos úteis que encontrou durante a semana)