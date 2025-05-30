# Progresso dos Estudos

## Semana 1: Fundamentos Práticos de LLMs e Embeddings

### Dia 1: Teoria dos LLMs
- [ ] Ler sobre LLMs (AWS Guide)
- [ ] Ler The Illustrated Transformer (50%)
- [ ] Resumir em 3 parágrafos
- [ ] Listar 5 aplicações práticas

### Dia 2: Teoria dos Embeddings  
- [ ] Ler sobre embeddings (OpenAI)
- [ ] Ler Word2Vec Explained
- [ ] Criar mapa mental de tipos
- [ ] Pensar em 3 casos de uso pessoais

### Dia 3: Setup e Primeiro Código
- [ ] Configurar ambiente Python
- [ ] Criar exemplo_01_basico.py
- [ ] Testar com 3-5 frases
- [ ] Documentar observações

### Dia 4: Comparação de Similaridade
- [ ] Criar exemplo_02_similaridade.py
- [ ] Testar pares similares vs diferentes
- [ ] Criar tabela de resultados
- [ ] Documentar insights

### Dia 5: Comparação de Modelos
- [ ] Criar exemplo_03_comparacao_modelos.py
- [ ] Testar 3 modelos diferentes
- [ ] Comparar velocidade vs qualidade
- [ ] Análise de trade-offs

### Dia 6: Visualização
- [ ] Criar exemplo_04_visualizacao.py
- [ ] Implementar t-SNE/UMAP
- [ ] Plotar embeddings
- [ ] Interpretar clusters

### Dia 7: Mini-Projeto Final
- [ ] Criar mini_projeto_busca_semantica.py
- [ ] Dataset de 20-30 frases
- [ ] Interface de busca
- [ ] README documentado

---

## Semana 2: Bancos Vetoriais na Prática

### Dia 1: Teoria dos Bancos Vetoriais
- [ ] Ler sobre bancos vetoriais e casos de uso
- [ ] Comparar ChromaDB, Pinecone, Weaviate, Qdrant
- [ ] Entender arquiteturas e trade-offs

### Dia 2: ChromaDB Setup
- [ ] Instalar e configurar ChromaDB
- [ ] Criar primeira coleção
- [ ] Indexar embeddings básicos

### Dia 3: Operações CRUD
- [ ] Implementar inserção de documentos
- [ ] Busca por similaridade
- [ ] Atualização e deleção

### Dia 4: Otimização e Performance
- [ ] Testar diferentes configurações
- [ ] Medir performance de queries
- [ ] Otimizar índices

### Dia 5: Integração com Aplicações
- [ ] API REST para banco vetorial
- [ ] Interface web simples
- [ ] Testes de integração

### Dia 6: Comparação de Frameworks
- [ ] Testar FAISS alternativo
- [ ] Comparar performance e facilidade de uso
- [ ] Documentar escolhas

### Dia 7: Mini-Projeto Final
- [ ] Sistema de busca semântica completo
- [ ] Interface web funcional
- [ ] Documentação e testes

---

## Semana 3: Retrieval-Augmented Generation (RAG)

### Dia 1: Teoria e Arquitetura RAG
- [ ] Entender conceito de RAG
- [ ] Mapear componentes: Retrieval → Augmentation → Generation
- [ ] Casos de uso vs fine-tuning

### Dia 2: LangChain Fundamentals
- [ ] Setup LangChain
- [ ] Implementar pipeline básico de RAG
- [ ] Document loaders e text splitters

### Dia 3: LlamaIndex Fundamentals
- [ ] Setup LlamaIndex
- [ ] Comparar com LangChain
- [ ] Implementar RAG alternativo

### Dia 4: Chunking Strategies
- [ ] Testar diferentes estratégias de chunking
- [ ] Otimizar para qualidade de retrieval
- [ ] Melhores práticas

### Dia 5: Prompt Engineering para RAG
- [ ] Otimizar prompts para RAG
- [ ] Testar diferentes templates
- [ ] Avaliar qualidade das respostas

### Dia 6: Avaliação e Métricas
- [ ] Implementar métricas de avaliação
- [ ] Criar dataset de teste
- [ ] Dashboard de qualidade

### Dia 7: Mini-Projeto Final
- [ ] Sistema Q&A completo
- [ ] Interface Streamlit
- [ ] Avaliação automatizada

---

## Semana 4: Model Context Protocol (MCP) e Interoperabilidade

### Dia 1: Introdução ao MCP
- [ ] Entender conceito de MCP
- [ ] Vantagens para interoperabilidade
- [ ] Casos de uso práticos

### Dia 2: Arquitetura e Componentes
- [ ] Estudar especificação MCP
- [ ] Entender componentes: Context, Resources, Tools
- [ ] Fluxo de comunicação

### Dia 3: Primeiro Cliente MCP
- [ ] Implementar cliente MCP básico
- [ ] Conectar com servidor demo
- [ ] Testar comunicação

### Dia 4: Servidor MCP
- [ ] Implementar servidor próprio
- [ ] Expor dados via MCP
- [ ] Testar cliente-servidor

### Dia 5: Integração com LangChain
- [ ] Integrar MCP com LangChain
- [ ] Comparar com tools tradicionais
- [ ] Vantagens da padronização

### Dia 6: Multi-Framework
- [ ] Conectar LangChain + LlamaIndex via MCP
- [ ] Demonstrar interoperabilidade
- [ ] Medir overhead

### Dia 7: Mini-Projeto Final
- [ ] Ecosistema multi-serviços
- [ ] Comunicação via MCP
- [ ] Dashboard de monitoramento

---

## Semana 5: Memória, Contexto e Persistência

### Dia 1: Teoria da Memória em IA
- [ ] Tipos de memória: curto vs longo prazo
- [ ] Importância para agentes
- [ ] Estratégias de implementação

### Dia 2: Memória no LangChain
- [ ] Implementar diferentes tipos de memória
- [ ] ConversationBufferMemory vs VectorMemory
- [ ] Trade-offs de cada abordagem

### Dia 3: Persistência com Bancos Vetoriais
- [ ] Implementar memória com ChromaDB
- [ ] Busca semântica no histórico
- [ ] Estratégias de indexação

### Dia 4: Memória Hierárquica
- [ ] Sistema multi-camada
- [ ] Buffer + sessão + longo prazo
- [ ] Algoritmos de consolidação

### Dia 5: Perfis de Usuário
- [ ] Sistema de perfis personalizados
- [ ] Extração de preferências
- [ ] Privacy e segurança

### Dia 6: Memória com LlamaIndex
- [ ] Implementar com LlamaIndex
- [ ] Comparar abordagens
- [ ] Integração com índices

### Dia 7: Mini-Projeto Final
- [ ] Chatbot com memória avançada
- [ ] Interface Streamlit
- [ ] Dashboard de memória

---

## Semana 6: Fine Tuning e LoRA

### Dia 1: Teoria do Fine-Tuning
- [ ] Fine-tuning vs RAG vs Prompt Engineering
- [ ] Quando usar cada abordagem
- [ ] Custos e benefícios

### Dia 2: Introdução ao LoRA
- [ ] Entender técnica LoRA
- [ ] Matemática: Low-Rank Adaptation
- [ ] Vantagens vs full fine-tuning

### Dia 3: Primeiro Fine-Tuning
- [ ] Setup ambiente: transformers, peft
- [ ] Fine-tuning com modelo pequeno
- [ ] Comparar resultados

### Dia 4: LoRA com PEFT
- [ ] Implementar LoRA
- [ ] Configurar hiperparâmetros
- [ ] Otimizar uso de memória

### Dia 5: Quantização
- [ ] 8-bit e 4-bit quantization
- [ ] QLoRA implementation
- [ ] Trade-offs performance vs qualidade

### Dia 6: Dataset e Avaliação
- [ ] Preparar datasets próprios
- [ ] Métricas de avaliação
- [ ] Pipeline completo

### Dia 7: Mini-Projeto Final
- [ ] Fine-tuning especializado
- [ ] Caso de uso específico
- [ ] Interface de demonstração

---

## Semana 7: Agentes de IA e Orquestração

### Dia 1: Teoria dos Agentes
- [ ] Tipos de agentes: Reactive, Deliberative
- [ ] Agentes vs chatbots
- [ ] Taxonomia e aplicações

### Dia 2: LangChain Agents
- [ ] Primeiro agente funcional
- [ ] Tools: Calculator, Search, Custom
- [ ] Reasoning e tool selection

### Dia 3: Tools Customizadas
- [ ] Criar ferramentas personalizadas
- [ ] File operations, API calls
- [ ] Melhores práticas de design

### Dia 4: Introdução ao CrewAI
- [ ] Setup CrewAI
- [ ] Agentes colaborativos
- [ ] Comparar com LangChain

### Dia 5: Agentes com Memória
- [ ] Integrar memória com agentes
- [ ] Histórico de ações
- [ ] Aprendizado de preferências

### Dia 6: Debugging e Observabilidade
- [ ] Sistema de logging
- [ ] Métricas de performance
- [ ] Dashboard de monitoramento

### Dia 7: Mini-Projeto Final
- [ ] Assistente pessoal autônomo
- [ ] Múltiplas ferramentas
- [ ] Interface web completa

---

## Semana 8: Orquestração Avançada e Multi-Agentes

### Dia 1: Teoria Multi-Agentes
- [ ] Sistemas multi-agentes
- [ ] Padrões de comunicação
- [ ] Desafios de coordenação

### Dia 2: AutoGen Framework
- [ ] Setup AutoGen
- [ ] Conversação entre agentes
- [ ] Padrões de comunicação

### Dia 3: CrewAI Avançado
- [ ] Workflows complexos
- [ ] Dependências entre agentes
- [ ] Otimização de colaboração

### Dia 4: Protocolos de Comunicação
- [ ] Message passing
- [ ] Shared memory
- [ ] Event-driven communication

### Dia 5: LangGraph Workflows
- [ ] Graph-based workflows
- [ ] Decision nodes e routing
- [ ] Visualização de execução

### Dia 6: Monitoramento Multi-Agente
- [ ] Métricas distribuídas
- [ ] Dashboard tempo real
- [ ] Troubleshooting

### Dia 7: Mini-Projeto Final
- [ ] Sistema análise de dados
- [ ] Pipeline multi-agente
- [ ] Orquestração completa

---

## Semana 9: Deploy, Observabilidade e Avaliação

### Dia 1: Estratégias de Deploy
- [ ] API REST vs serverless vs edge
- [ ] Trade-offs de cada abordagem
- [ ] Escolha por caso de uso

### Dia 2: API com FastAPI
- [ ] API production-ready
- [ ] Endpoints robustos
- [ ] Middleware e documentação

### Dia 3: Containerização
- [ ] Docker otimizado
- [ ] Multi-stage builds
- [ ] docker-compose stack

### Dia 4: Observabilidade
- [ ] Métricas de performance
- [ ] Prometheus + Grafana
- [ ] Alertas automáticos

### Dia 5: Avaliação Contínua
- [ ] A/B testing
- [ ] Data drift detection
- [ ] Re-treinamento automático

### Dia 6: Otimização e Escala
- [ ] Caching e batch inference
- [ ] Load balancing
- [ ] Auto-scaling

### Dia 7: Mini-Projeto Final
- [ ] Plataforma ML completa
- [ ] Deploy em cloud
- [ ] Monitoramento em produção

---

## Semana 10: Tópicos Avançados e Multi-modalidade

### Dia 1: Introdução Multi-modalidade
- [ ] Modelos vision-language
- [ ] Modalidades: texto, imagem, áudio
- [ ] Arquiteturas de fusão

### Dia 2: Modelos Vision-Language
- [ ] GPT-4V, LLaVA, CLIP
- [ ] Image captioning
- [ ] Visual question answering

### Dia 3: Geração Multi-modal
- [ ] Texto para imagem
- [ ] Workflows complexos
- [ ] Avaliação de qualidade

### Dia 4: Segurança e Guardrails
- [ ] Content filtering
- [ ] Detecção de toxicidade
- [ ] Framework de segurança

### Dia 5: Prompt Injection
- [ ] Tipos de ataques
- [ ] Defesas e mitigações
- [ ] Red team testing

### Dia 6: Avaliação Ética
- [ ] Métricas de bias
- [ ] Fairness e transparência
- [ ] Pipeline ético

### Dia 7: Mini-Projeto Final
- [ ] Assistente multi-modal seguro
- [ ] Sistema de guardrails
- [ ] Auditoria completa

---

## Observações Gerais
- **Data de início:** ___________
- **Dificuldades encontradas:**
- **Aprendizados importantes:**
- **Ideias para projetos futuros:**
- **Tecnologias favoritas:**
- **Próximos passos após as 10 semanas:** 