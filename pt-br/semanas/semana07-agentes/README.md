# Semana 7: Agentes de IA e Orquestração

## 🎯 Objetivo Geral
Dominar conceitos e implementação de agentes de IA autônomos, incluindo diferentes tipos de agentes, ferramentas, e frameworks como LangChain Agents e CrewAI.

---

## 📅 Cronograma Diário (7 dias)

### **Dia 1: Teoria dos Agentes de IA**
**Tempo:** 30-45 min  
**Objetivo:** Entender o que são agentes e sua classificação

**Atividades:**
- [ ] 📖 Ler: [What are AI Agents?](https://python.langchain.com/docs/tutorials/agents/)
- [ ] 📖 Read: [Types of AI Agents](https://cloud.google.com/discover/what-are-ai-agents)
- [ ] 📝 Mapear tipos: Reactive, Deliberative, Hybrid, Learning
- [ ] 🧠 Listar 5 exemplos de agentes no mundo real
- [ ] 📝 Comparar agentes vs chatbots tradicionais

**Resultado esperado:** Compreensão sólida da taxonomia de agentes

---

### **Dia 2: LangChain Agents Básico**
**Tempo:** 45-60 min  
**Objetivo:** Implementar primeiro agente com LangChain

**Atividades:**
- [ ] 📖 Ler: [LangChain Agents Guide](https://python.langchain.com/docs/how_to/#agents)
- [ ] 👨‍💻 Criar `exemplo_01_agente_basico.py`
- [ ] 🧪 Implementar agente com tools:
  - Calculator tool
  - Search tool
  - Custom tool simples
- [ ] 📊 Testar reasoning e tool selection
- [ ] 📝 Documentar comportamento do agente

**Resultado esperado:** Primeiro agente funcional com ferramentas

---

### **Dia 3: Tools Customizadas**
**Tempo:** 45-60 min  
**Objetivo:** Criar ferramentas personalizadas para agentes

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_02_custom_tools.py`
- [ ] 🛠️ Implementar tools personalizadas:
  - File reader/writer
  - API caller
  - Database query tool
  - Email sender
- [ ] 🧪 Testar agente com workflow complexo
- [ ] 📊 Analisar como agente escolhe ferramentas
- [ ] 📝 Melhores práticas para design de tools

**Resultado esperado:** Biblioteca de ferramentas reutilizáveis

---

### **Dia 4: Introdução ao CrewAI**
**Tempo:** 45-60 min  
**Objetivo:** Explorar framework CrewAI para agentes colaborativos

**Atividades:**
- [ ] 📖 Ler: [CrewAI Documentation](https://docs.crewai.com/)
- [ ] 👨‍💻 Criar `exemplo_03_crewai_basico.py`
- [ ] 🧪 Implementar crew simples:
  - Research agent
  - Writer agent
  - Editor agent
- [ ] 📊 Comparar com LangChain agents
- [ ] 📝 Documentar vantagens/desvantagens de cada framework

**Resultado esperado:** Domínio básico do CrewAI

---

### **Dia 5: Agentes com Memória**
**Tempo:** 45-60 min  
**Objetivo:** Integrar sistema de memória com agentes

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_04_agente_memoria.py`
- [ ] 🧠 Implementar agente com:
  - Memória de conversação
  - Histórico de ações
  - Aprendizado de preferências
- [ ] 🧪 Testar persistência entre sessões
- [ ] 📊 Validar melhoria de performance com memória
- [ ] 📝 Estratégias de otimização de memória para agentes

**Resultado esperado:** Agente com memória persistente funcional

---

### **Dia 6: Debugging e Observabilidade**
**Tempo:** 45-60 min  
**Objetivo:** Implementar ferramentas de debugging e monitoramento

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_05_debugging_agentes.py`
- [ ] 🔍 Implementar logging detalhado:
  - Decision traces
  - Tool usage metrics
  - Error handling
- [ ] 📊 Dashboard simples para monitoramento
- [ ] 🧪 Testar com casos de erro
- [ ] 📝 Checklist de debugging para agentes

**Resultado esperado:** Sistema robusto de observabilidade

---

### **Dia 7: Mini-Projeto Final**
**Tempo:** 60-90 min  
**Objetivo:** Sistema de agentes para automação complexa

**Atividades:**
- [ ] 👨‍💻 Criar `mini_projeto_assistente_pessoal/`
- [ ] 🏗️ Implementar assistente com capacidades:
  - Gerenciamento de emails
  - Pesquisa e sumarização
  - Agendamento de tarefas
  - Relatórios automáticos
- [ ] 🔧 Features avançadas:
  - Múltiplas ferramentas integradas
  - Memória persistente
  - Interface web intuitiva
  - Sistema de logs completo
- [ ] 📊 Dashboard de atividades do agente
- [ ] 📝 README com casos de uso e exemplos
- [ ] 🎉 Demo completa funcionando

**Resultado esperado:** Assistente pessoal autônomo e funcional

---

## 📚 Recursos de Estudo

### **Leituras Essenciais**
- [LangChain Agents](https://python.langchain.com/docs/how_to/#agents)
- [CrewAI Documentation](https://docs.crewai.com/)
- [AI Agents Explained](https://python.langchain.com/docs/tutorials/agents/)

### **Leituras Complementares**
- [AutoGPT Architecture](https://github.com/Significant-Gravitas/AutoGPT)
- [Agent Memory Systems](https://blog.langchain.dev/memory-for-agents/)
- [Multi-Agent Frameworks Comparison](https://medium.com/@cognidownunder/in-the-ever-evolving-world-of-ai-frameworks-two-contenders-have-risen-to-prominence-each-vying-ee511ca7a366)

### **Papers Relevantes**
- [ReAct: Reasoning and Acting with LLMs](https://arxiv.org/abs/2210.03629)
- [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366)

---

## 🛠️ Setup Técnico

### **Dependências**
```bash
# Adicionar ao requirements.txt
langchain==0.0.340
crewai==0.1.55
openai==1.3.5
google-search-results==2.4.2
streamlit==1.28.2
plotly==5.17.0
sqlite3  # Built-in
requests==2.31.0
beautifulsoup4==4.12.2
python-dotenv==1.0.0
```

### **Estrutura de Arquivos**
```
semana07-agentes/
├── notas.md                          # Este arquivo
├── experimentos.md                   # Suas anotações
├── exemplos/
│   ├── exemplo_01_agente_basico.py
│   ├── exemplo_02_custom_tools.py
│   ├── exemplo_03_crewai_basico.py
│   ├── exemplo_04_agente_memoria.py
│   └── exemplo_05_debugging_agentes.py
└── mini-projeto/
    ├── mini_projeto_assistente_pessoal/
    │   ├── app.py                    # Interface principal
    │   ├── agents/                   # Agentes especializados
    │   ├── tools/                    # Ferramentas customizadas
    │   ├── memory/                   # Sistema de memória
    │   ├── monitoring/               # Logs e métricas
    │   └── config/                   # Configurações
    └── README.md
```

---

## ✅ Checklist de Aprendizado

### **Conceitos Teóricos**
- [ ] Entendo diferenças entre tipos de agentes
- [ ] Sei quando usar LangChain vs CrewAI
- [ ] Compreendo arquitetura ReAct
- [ ] Conheço limitações e desafios dos agentes

### **Habilidades Práticas**
- [ ] Implementei agente básico com LangChain
- [ ] Criei ferramentas personalizadas
- [ ] Usei CrewAI para agentes colaborativos
- [ ] Integrei memória com agentes
- [ ] Implementei sistema de debugging

### **Projeto Final**
- [ ] Assistente pessoal multi-funcional
- [ ] Interface web intuitiva
- [ ] Sistema de monitoramento
- [ ] Múltiplas ferramentas integradas
- [ ] Documentação completa

---

## 📝 Espaço para Anotações

### **Comparação de Frameworks**
- **LangChain Agents:**
  - Prós:
  - Contras:
  - Melhor para:

- **CrewAI:**
  - Prós:
  - Contras:
  - Melhor para:

### **Ferramentas Mais Úteis**
- Calculator:
- Search:
- File operations:
- API calls:

### **Padrões de Design**
- Tool selection strategies:
- Error handling:
- Memory management:

### **Problemas Comuns**
- (Erros frequentes e soluções)

### **Ideias de Melhorias**
- (Próximas funcionalidades a implementar) 