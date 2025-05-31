# Week 6: Fine-Tuning and LoRA

## 🎯 General Objective
Master fine-tuning techniques and LoRA (Low-Rank Adaptation) to adapt pre-trained models to specific needs, including quantization and model optimization.

---

## 📅 Daily Schedule (7 days)

### **Day 1: Fine-Tuning Theory**
**Time:** 30-45 min  
**Objective:** Understand fundamental fine-tuning concepts vs other approaches

**Activities:**
- [ ] 📖 Read: [Fine-tuning vs RAG vs Prompt Engineering](https://python.langchain.com/docs/tutorials/rag/)
- [ ] 📖 Read: [When to Fine-tune](https://platform.openai.com/docs/guides/fine-tuning)
- [ ] 📝 Summarize: When to use fine-tuning, RAG, or prompt engineering
- [ ] 🧠 List 5 ideal scenarios for fine-tuning
- [ ] 📝 Map costs and benefits of each approach

**Expected outcome:** Clear understanding of when to apply fine-tuning

---

### **Day 2: Introduction to LoRA**
**Time:** 45-60 min  
**Objective:** Understand LoRA technique and its advantages

**Activities:**
- [ ] 📖 Read: [LoRA Paper](https://arxiv.org/abs/2106.09685)
- [ ] 📖 Read: [LoRA Explained Simply](https://www.cloudflare.com/pt-br/learning/ai/what-is-lora/)
- [ ] 📝 Draw LoRA architecture diagram
- [ ] 🧠 Understand math: A + BA where A,B are low-rank matrices
- [ ] 📝 Compare LoRA vs full fine-tuning: memory, time, quality

**Expected outcome:** Conceptual mastery of LoRA technique

---

### **Day 3: Setup and First Fine-Tuning**
**Time:** 45-60 min  
**Objective:** Configure environment and execute first fine-tuning

**Activities:**
- [ ] ⚙️ Setup environment: transformers, peft, bitsandbytes
- [ ] 👨‍💻 Create `example_01_basic_fine_tuning.py`
- [ ] 🧪 Simple fine-tuning with small model (GPT-2 or DistilGPT-2)
- [ ] 📊 Compare original vs fine-tuned model
- [ ] 📝 Document process and results

**Expected outcome:** First working fine-tuning

---

### **Day 4: LoRA with HuggingFace PEFT**
**Time:** 45-60 min  
**Objective:** Implement LoRA using PEFT library

**Activities:**
- [ ] 👨‍💻 Create `example_02_lora_peft.py`
- [ ] 🧪 Apply LoRA to larger model (Llama 2 7B or similar)
- [ ] ⚙️ Configure hyperparameters: rank, alpha, dropout
- [ ] 📊 Compare memory usage: full vs LoRA
- [ ] 📝 Document optimal configurations found

**Expected outcome:** LoRA working with production model

---

### **Day 5: Quantization and Optimization**
**Time:** 45-60 min  
**Objective:** Apply quantization techniques to optimize models

**Activities:**
- [ ] 👨‍💻 Create `example_03_quantization.py`
- [ ] 🧪 Test different techniques:
  - 8-bit quantization
  - 4-bit quantization (QLoRA)
  - GPTQ quantization
- [ ] 📊 Compare: speed, memory, quality
- [ ] 🔍 Identify trade-offs for each technique
- [ ] 📝 Guide on when to use each quantization type

**Expected outcome:** Expertise in model optimization

---

### **Day 6: Dataset Preparation and Evaluation**
**Time:** 45-60 min  
**Objective:** Prepare custom datasets and evaluate fine-tuning quality

**Activities:**
- [ ] 👨‍💻 Create `example_04_dataset_preparation.py`
- [ ] 📚 Prepare custom dataset (chat, classification, or generation)
- [ ] 🧪 Implement evaluation metrics:
  - Perplexity
  - BLEU/ROUGE (if applicable)
  - Accuracy (for classification)
- [ ] 📊 Compare performance before/after fine-tuning
- [ ] 📝 Document best practices for data preparation

**Expected outcome:** Complete preparation and evaluation pipeline

---

### **Day 7: Final Mini-Project**
**Time:** 60-90 min  
**Objective:** Complete fine-tuning for specific use case

**Activities:**
- [ ] 👨‍💻 Create `mini_specialized_fine_tuning_project/`
- [ ] 🎯 Choose specific use case:
  - Domain-specialized chatbot
  - Code generator
  - Text classifier
- [ ] 🏗️ Complete pipeline:
  - Data collection/preparation
  - Fine-tuning with LoRA
  - Quantization for deployment
  - Testing interface
- [ ] 📊 Metrics dashboard and comparisons
- [ ] 📝 Detailed README with results and analysis
- [ ] 🎉 Working demo + improvement analysis

**Expected outcome:** Production-ready fine-tuned model

---

## 📚 Study Resources

### **Essential Readings**
- [LoRA Paper](https://arxiv.org/abs/2106.09685)
- [HuggingFace PEFT](https://github.com/huggingface/peft)
- [Fine-tuning Best Practices](https://huggingface.co/docs/transformers/en/training)

### **Additional Readings**
- [QLoRA Paper](https://arxiv.org/abs/2305.14314)
- [AdaLoRA: Adaptive Budget Allocation](https://arxiv.org/abs/2303.10512)
- [DoRA: Weight-Decomposed Low-Rank Adaptation](https://arxiv.org/abs/2402.09353)

### **Practical Tutorials**
- [Fine-tuning Llama 2 with LoRA](https://medium.com/@harsh.vardhan7695/fine-tuning-llama-2-using-lora-and-qlora-a-comprehensive-guide-fd2260f0aa5f)
- [PEFT Documentation](https://huggingface.co/docs/peft/index)
- [Quantization Guide](https://huggingface.co/docs/transformers/quantization)

---

## 🛠️ Technical Setup

### **Dependencies**
```bash
# Add to requirements.txt
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

### **File Structure**
```
week06-fine-tuning/
├── README.md                         # This file
├── experiments.md                    # Your notes
├── examples/
│   ├── example_01_basic_fine_tuning.py
│   ├── example_02_lora_peft.py
│   ├── example_03_quantization.py
│   └── example_04_dataset_preparation.py
└── mini-project/
    ├── mini_specialized_fine_tuning_project/
    │   ├── train.py                  # Training script
    │   ├── inference.py              # Inference script
    │   ├── evaluate.py               # Model evaluation
    │   ├── data_prep.py              # Data preparation
    │   ├── app.py                    # Demo interface
    │   ├── configs/                  # Configurations
    │   └── models/                   # Saved models
    └── README.md
```

---

## ✅ Learning Checklist

### **Theoretical Concepts**
- [ ] I understand differences: fine-tuning vs RAG vs prompt engineering
- [ ] I comprehend LoRA math and intuition
- [ ] I know when to apply quantization
- [ ] I know trade-offs of each technique

### **Practical Skills**
- [ ] I executed complete fine-tuning
- [ ] I implemented LoRA with PEFT
- [ ] I applied 4-bit and 8-bit quantization
- [ ] I prepared custom datasets
- [ ] I evaluated model quality

### **Final Project**
- [ ] Specialized fine-tuned model
- [ ] Complete training pipeline
- [ ] Evaluation and metrics
- [ ] Deployment-ready optimization

---

## 📝 Space for Notes

### **Approach Comparison**
- **Fine-tuning:** Best for:
- **RAG:** Best for:
- **Prompt Engineering:** Best for:

### **LoRA Configuration**
- Optimal rank:
- Best alpha value:
- Dropout rate:

### **Quantization Results**
- 8-bit performance:
- 4-bit performance:
- Memory savings:

### **Best Practices Discovered**
- Dataset preparation:
- Training optimization:
- Evaluation metrics:

### **Production Considerations**
- Deployment requirements:
- Performance optimization:
- Cost considerations: 