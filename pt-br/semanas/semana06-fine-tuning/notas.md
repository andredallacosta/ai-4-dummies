# Semana 6: Fine Tuning e LoRA

## 🎯 Objetivo Geral
Dominar técnicas de fine-tuning e LoRA (Low-Rank Adaptation) para adaptar modelos pré-treinados às necessidades específicas, incluindo quantização e otimização de modelos.

---

## 📅 Cronograma Diário (7 dias)

### **Dia 1: Teoria do Fine-Tuning**
**Tempo:** 30-45 min  
**Objetivo:** Entender conceitos fundamentais de fine-tuning vs outras abordagens

**Atividades:**
- [ ] 📖 Ler: [Fine-tuning vs RAG vs Prompt Engineering](https://blog.langchain.dev/fine-tuning-vs-retrieval-augmented-generation/)
- [ ] 📖 Ler: [When to Fine-tune](https://platform.openai.com/docs/guides/fine-tuning/when-to-use-fine-tuning)
- [ ] 📝 Resumir: Quando usar fine-tuning, RAG ou prompt engineering
- [ ] 🧠 Listar 5 cenários ideais para fine-tuning
- [ ] 📝 Mapear custos e benefícios de cada abordagem

**Resultado esperado:** Compreensão clara de quando aplicar fine-tuning

---

### **Dia 2: Introdução ao LoRA**
**Tempo:** 45-60 min  
**Objetivo:** Entender a técnica LoRA e suas vantagens

**Atividades:**
- [ ] 📖 Ler: [LoRA Paper](https://arxiv.org/abs/2106.09685)
- [ ] 📖 Ler: [LoRA Explained Simply](https://blog.paperspace.com/lora-explained/)
- [ ] 📝 Desenhar diagrama da arquitetura LoRA
- [ ] 🧠 Entender matemática: A + BA onde A,B são matrizes de rank baixo
- [ ] 📝 Comparar LoRA vs full fine-tuning: memória, tempo, qualidade

**Resultado esperado:** Domínio conceitual da técnica LoRA

---

### **Dia 3: Setup e Primeiro Fine-Tuning**
**Tempo:** 45-60 min  
**Objetivo:** Configurar ambiente e executar primeiro fine-tuning

**Atividades:**
- [ ] ⚙️ Setup ambiente: transformers, peft, bitsandbytes
- [ ] 👨‍💻 Criar `exemplo_01_fine_tuning_basico.py`
- [ ] 🧪 Fine-tuning simples com modelo pequeno (GPT-2 ou DistilGPT-2)
- [ ] 📊 Comparar modelo original vs fine-tuned
- [ ] 📝 Documentar processo e resultados

**Resultado esperado:** Primeiro fine-tuning funcionando

---

### **Dia 4: LoRA com HuggingFace PEFT**
**Tempo:** 45-60 min  
**Objetivo:** Implementar LoRA usando biblioteca PEFT

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_02_lora_peft.py`
- [ ] 🧪 Aplicar LoRA em modelo maior (Llama 2 7B ou similar)
- [ ] ⚙️ Configurar hiperparâmetros: rank, alpha, dropout
- [ ] 📊 Comparar uso de memória: full vs LoRA
- [ ] 📝 Documentar configurações ótimas encontradas

**Resultado esperado:** LoRA funcionando com modelo de produção

---

### **Dia 5: Quantização e Otimização**
**Tempo:** 45-60 min  
**Objetivo:** Aplicar técnicas de quantização para otimizar modelos

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_03_quantizacao.py`
- [ ] 🧪 Testar diferentes técnicas:
  - 8-bit quantization
  - 4-bit quantization (QLoRA)
  - GPTQ quantization
- [ ] 📊 Comparar: velocidade, memória, qualidade
- [ ] 🔍 Identificar trade-offs para cada técnica
- [ ] 📝 Guia de quando usar cada tipo de quantização

**Resultado esperado:** Expertise em otimização de modelos

---

### **Dia 6: Dataset Preparation e Avaliação**
**Tempo:** 45-60 min  
**Objetivo:** Preparar datasets próprios e avaliar qualidade do fine-tuning

**Atividades:**
- [ ] 👨‍💻 Criar `exemplo_04_dataset_preparation.py`
- [ ] 📚 Preparar dataset personalizado (chat, classificação, ou geração)
- [ ] 🧪 Implementar métricas de avaliação:
  - Perplexity
  - BLEU/ROUGE (se aplicável)
  - Accuracy (para classificação)
- [ ] 📊 Comparar performance antes/depois do fine-tuning
- [ ] 📝 Documentar melhores práticas para preparação de dados

**Resultado esperado:** Pipeline completo de preparação e avaliação

---

### **Dia 7: Mini-Projeto Final**
**Tempo:** 60-90 min  
**Objetivo:** Fine-tuning completo para caso de uso específico

**Atividades:**
- [ ] 👨‍💻 Criar `mini_projeto_fine_tuning_especializado/`
- [ ] 🎯 Escolher caso de uso específico:
  - Chatbot especializado em domínio
  - Gerador de código
  - Classificador de texto
- [ ] 🏗️ Pipeline completo:
  - Coleta/preparação de dados
  - Fine-tuning com LoRA
  - Quantização para deployment
  - Interface de teste
- [ ] 📊 Dashboard de métricas e comparações
- [ ] 📝 README detalhado com resultados e análises
- [ ] 🎉 Demo funcionando + análise de melhorias

**Resultado esperado:** Modelo fine-tuned pronto para produção

---

## 📚 Recursos de Estudo

### **Leituras Essenciais**
- [LoRA Paper](https://arxiv.org/abs/2106.09685)
- [HuggingFace PEFT](https://github.com/huggingface/peft)
- [Fine-tuning Best Practices](https://blog.paperspace.com/fine-tuning-transformers/)

### **Leituras Complementares**
- [QLoRA Paper](https://arxiv.org/abs/2305.14314)
- [AdaLoRA: Adaptive Budget Allocation](https://arxiv.org/abs/2303.10512)
- [DoRA: Weight-Decomposed Low-Rank Adaptation](https://arxiv.org/abs/2402.09353)

### **Tutoriais Práticos**
- [Fine-tuning Llama 2 with LoRA](https://blog.paperspace.com/fine-tune-llama-2-with-lora/)
- [PEFT Documentation](https://huggingface.co/docs/peft/index)
- [Quantization Guide](https://huggingface.co/docs/transformers/quantization)

---

## 🛠️ Setup Técnico

### **Dependências**
```bash
# Adicionar ao requirements.txt
transformers==4.36.0
peft==0.7.1
bitsandbytes==0.41.3
datasets==2.15.0
accelerate==0.25.0
torch>=2.0.0
trl==0.7.4
wandb==0.16.1
scipy==1.11.4
scikit-learn==1.3.2
```

### **Estrutura de Arquivos**
```
semana06-fine-tuning/
├── notas.md                          # Este arquivo
├── experimentos.md                   # Suas anotações
├── exemplos/
│   ├── exemplo_01_fine_tuning_basico.py
│   ├── exemplo_02_lora_peft.py
│   ├── exemplo_03_quantizacao.py
│   └── exemplo_04_dataset_preparation.py
└── mini-projeto/
    ├── mini_projeto_fine_tuning_especializado/
    │   ├── train.py                  # Script de treinamento
    │   ├── inference.py              # Script de inferência
    │   ├── evaluate.py               # Avaliação de modelos
    │   ├── data_prep.py              # Preparação de dados
    │   ├── app.py                    # Interface demo
    │   ├── configs/                  # Configurações
    │   └── models/                   # Modelos salvos
    └── README.md
```

---

## ✅ Checklist de Aprendizado

### **Conceitos Teóricos**
- [ ] Entendo diferenças: fine-tuning vs RAG vs prompt engineering
- [ ] Compreendo matemática e intuição do LoRA
- [ ] Sei quando aplicar quantização
- [ ] Conheço trade-offs de cada técnica

### **Habilidades Práticas**
- [ ] Executei fine-tuning completo
- [ ] Implementei LoRA com PEFT
- [ ] Apliquei quantização 4-bit e 8-bit
- [ ] Preparei datasets personalizados
- [ ] Avaliei qualidade de modelos fine-tuned

### **Projeto Final**
- [ ] Modelo fine-tuned para caso específico
- [ ] Pipeline de treinamento otimizado
- [ ] Interface de demonstração
- [ ] Métricas de avaliação implementadas
- [ ] Documentação técnica completa

---

## 📝 Espaço para Anotações

### **Comparação de Técnicas**
- **Full Fine-tuning:**
  - Prós:
  - Contras:
  - Quando usar:

- **LoRA:**
  - Prós:
  - Contras:
  - Hiperparâmetros ótimos:

### **Configurações que Funcionaram**
- Rank ótimo:
- Alpha ideal:
- Learning rate:
- Batch size:

### **Resultados de Quantização**
- 8-bit: Speedup X, Memória Y%, Qualidade Z%
- 4-bit: Speedup X, Memória Y%, Qualidade Z%

### **Lições Aprendidas**
- (Problemas encontrados e soluções)

### **Ideias para Próximos Projetos**
- (Aplicações de fine-tuning que poderiam explorar) 