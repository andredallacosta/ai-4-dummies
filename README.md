# Estudos e Projetos em IA Generativa, RAG, Agentes e Orquestração

Este repositório documenta uma jornada completa de estudos e experimentos práticos com IA generativa, RAG, agentes, bancos vetoriais e as principais ferramentas do mercado.

## 🎯 Sobre o Projeto

Um plano estruturado de **10 semanas** cobrindo desde fundamentos até tópicos avançados, com foco em **implementação prática** e projetos reais. Cada semana inclui teoria, prática e um mini-projeto final.

## 📚 Plano de Estudo Completo

O plano detalhado está em [`plano_ia_generativa.md`](plano_ia_generativa.md).

### 📅 Cronograma das Semanas

| Semana | Tópico | Status | Mini-Projeto |
|--------|--------|--------|--------------|
| **1** | [Fundamentos de LLMs e Embeddings](semanas/semana01-llms-embeddings/) | ✅ | Sistema de busca semântica |
| **2** | [Bancos Vetoriais na Prática](semanas/semana02-bancos-vetoriais/) | 🔄 | Busca semântica com ChromaDB |
| **3** | [Retrieval-Augmented Generation (RAG)](semanas/semana03-rag/) | ✅ | Q&A system completo |
| **4** | [Model Context Protocol (MCP)](semanas/semana04-mcp/) | ✅ | Ecosistema distribuído |
| **5** | [Memória e Persistência](semanas/semana05-memoria/) | ✅ | Chatbot com memória avançada |
| **6** | [Fine Tuning e LoRA](semanas/semana06-fine-tuning/) | ✅ | Modelo especializado |
| **7** | [Agentes de IA](semanas/semana07-agentes/) | ✅ | Assistente pessoal autônomo |
| **8** | [Multi-Agentes e Orquestração](semanas/semana08-multi-agentes/) | ✅ | Sistema análise de dados |
| **9** | [Deploy e Observabilidade](semanas/semana09-deploy/) | ✅ | Plataforma ML em produção |
| **10** | [Tópicos Avançados e Multi-modalidade](semanas/semana10-avancados/) | ✅ | Assistente multi-modal seguro |

## 🚀 Progresso e Acompanhamento

Acompanhe o progresso detalhado em [`progresso.md`](progresso.md) com checklists diários e anotações.

## 📁 Estrutura do Repositório

```
awesome-ai-pocs/
├── README.md                          # Este arquivo
├── plano_ia_generativa.md            # Plano completo de estudos
├── progresso.md                      # Acompanhamento do progresso
├── requirements.txt                  # Dependências consolidadas
├── LICENSE                          # Licença MIT
│
├── semanas/                         # Uma pasta por semana
│   ├── semana01-llms-embeddings/
│   │   ├── notas.md                 # Teoria e cronograma
│   │   ├── experimentos.md          # Anotações práticas
│   │   ├── exemplos/                # Scripts de exemplo
│   │   └── mini-projeto/            # Projeto final da semana
│   ├── semana02-bancos-vetoriais/
│   ├── semana03-rag/
│   ├── semana04-mcp/
│   ├── semana05-memoria/
│   ├── semana06-fine-tuning/
│   ├── semana07-agentes/
│   ├── semana08-multi-agentes/
│   ├── semana09-deploy/
│   └── semana10-avancados/
│
├── projetos/                        # Projetos independentes maiores
├── imagens/                         # Assets e imagens
└── venv/                            # Ambiente virtual Python
```

## 🛠️ Tecnologias e Ferramentas Cobertas

### **Frameworks de IA**
- **LangChain** - Desenvolvimento de aplicações com LLMs
- **LlamaIndex** - Indexação e busca inteligente
- **CrewAI** - Agentes colaborativos
- **AutoGen** - Sistemas multi-agentes

### **Bancos Vetoriais**
- **ChromaDB** - Banco vetorial local
- **Pinecone** - Banco vetorial na nuvem
- **FAISS** - Busca de similaridade eficiente
- **Qdrant** - Motor de busca vetorial

### **Modelos e APIs**
- **OpenAI** (GPT-4, GPT-3.5, DALL-E, Embeddings)
- **HuggingFace** (Transformers, PEFT, Datasets)
- **Sentence Transformers** - Embeddings especializados

### **Deployment e Produção**
- **FastAPI** - APIs robustas
- **Docker** - Containerização
- **Streamlit/Gradio** - Interfaces web
- **Prometheus/Grafana** - Monitoramento

### **Tópicos Avançados**
- **Fine-tuning** com LoRA e quantização
- **Model Context Protocol** (MCP)
- **Multi-modalidade** (texto, imagem, áudio)
- **Segurança** e guardrails
- **MLOps** e observabilidade

## 🚀 Como Começar

### 1. **Clone o repositório**
```bash
git clone https://github.com/seu-usuario/awesome-ai-pocs.git
cd awesome-ai-pocs
```

### 2. **Configure o ambiente**
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
# ou
venv\Scripts\activate     # Windows

pip install -r requirements.txt
```

### 3. **Configure suas API keys**
```bash
cp .env.example .env
# Edite .env com suas chaves da OpenAI, etc.
```

### 4. **Comece pela Semana 1**
```bash
cd semanas/semana01-llms-embeddings/
# Leia notas.md e siga o cronograma
```

## 💡 Como Usar Este Repositório

### **Para Estudantes**
- Siga o cronograma das semanas sequencialmente
- Complete os exercícios práticos diários
- Implemente os mini-projetos
- Use `experimentos.md` para anotar descobertas

### **Para Instrutores**
- Use como currículo estruturado
- Adapte os cronogramas conforme necessário
- Compartilhe os mini-projetos como referência

### **Para Profissionais**
- Foque nas semanas mais relevantes ao seu trabalho
- Use os mini-projetos como base para projetos reais
- Contribua com melhorias e novos casos de uso

## 🤝 Contribuindo

Contribuições são muito bem-vindas! Algumas formas de contribuir:

- **🐛 Report bugs** ou problemas nos exemplos
- **📚 Melhore a documentação** com mais explicações
- **💡 Sugira novos tópicos** ou tecnologias
- **🔧 Contribua com código** melhorando exemplos
- **📖 Compartilhe experiências** nos issues

## 📈 Roadmap Futuro

- [ ] **Semana 11**: LLMs locais (Ollama, GPT4All)
- [ ] **Semana 12**: Integração com ferramentas (Zapier, n8n)
- [ ] **Semana 13**: IA para código (GitHub Copilot, CodeT5)
- [ ] **Semana 14**: Compliance e governança de IA
- [ ] **Projetos especiais**: Integrações enterprise

## 📄 Licença

Este projeto está sob a licença MIT. Veja [LICENSE](LICENSE) para mais detalhes.

## 🌟 Agradecimentos

Inspirado pelas melhores práticas da comunidade de IA e Machine Learning. Agradecimentos especiais às comunidades do LangChain, LlamaIndex, HuggingFace e OpenAI.

---

**⭐ Se este repositório te ajudou, considere dar uma estrela!**

**📢 Compartilhe com sua equipe e rede profissional!**

**🔔 Watch o repositório para acompanhar atualizações!** 