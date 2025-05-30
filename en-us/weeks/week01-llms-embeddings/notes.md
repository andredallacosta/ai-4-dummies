# Week 1: Practical Fundamentals of LLMs and Embeddings

## 🎯 General Objective
Understand in theory and practice what LLMs and embeddings are, how to generate them and use them for real semantic similarity tasks.

---

## 📅 Daily Schedule (7 days)

### **Day 1: LLM Theory**
**Time:** 30-45 min  
**Objective:** Understand the current LLM landscape

**Activities:**
- [ ] 📖 Read: [What are Large Language Models (LLMs)?](https://aws.amazon.com/what-is/large-language-model/)
- [ ] 📖 Read: [The Illustrated Transformer](http://jalammar.github.io/illustrated-transformer/) (first 50%)
- [ ] 📝 Summarize in 3 paragraphs: What are LLMs and why they are important
- [ ] 🧠 List 5 practical LLM applications you know

**Expected result:** Basic vocabulary about LLMs and transformers

---

### **Day 2: Embedding Theory**
**Time:** 30-45 min  
**Objective:** Understand the concept of embeddings and their applications

**Activities:**
- [ ] 📖 Read: [What are embeddings?](https://platform.openai.com/docs/guides/embeddings/what-are-embeddings)
- [ ] 📖 Read: [Word2Vec Explained](https://towardsdatascience.com/word2vec-explained-49c52b4ccb71)
- [ ] 📝 Create a mind map: types of embeddings (word, sentence, document)
- [ ] 🧠 Think of 3 use cases for embeddings in your professional/personal context

**Expected result:** Clear understanding of how embeddings capture meaning

---

### **Day 3: Setup and First Code**
**Time:** 45-60 min  
**Objective:** Configure environment and generate first embeddings

**Activities:**
- [ ] ⚙️ Python environment setup (requirements.txt)
- [ ] 👨‍💻 Create `example_01_basic.py`: Generate embeddings with Sentence Transformers
- [ ] 🧪 Test with 3-5 simple sentences
- [ ] 📊 Print dimensions and first values of embeddings
- [ ] 📝 Document observations in `experiments.md` file

**Expected result:** Working environment + first embeddings generated

---

### **Day 4: Similarity Comparison**
**Time:** 45-60 min  
**Objective:** Calculate and interpret semantic similarity

**Activities:**
- [ ] 👨‍💻 Create `example_02_similarity.py`: calculate cosine similarity
- [ ] 🧪 Test with sentence pairs: similar vs different
- [ ] 📊 Create a results table (sentence1, sentence2, similarity)
- [ ] 🔍 Investigate: Why do some sentences have high similarity?
- [ ] 📝 Document insights about limitations and surprises

**Expected result:** Practical understanding of how to measure semantic similarity

---

### **Day 5: Model Comparison**
**Time:** 45-60 min  
**Objective:** Test different embedding models

**Activities:**
- [ ] 👨‍💻 Create `example_03_model_comparison.py`
- [ ] 🧪 Test at least 3 models: 
  - `all-MiniLM-L6-v2` (fast)
  - `all-mpnet-base-v2` (better quality)
  - `distilbert-base-multilingual-cased` (multilingual)
- [ ] 📊 Compare similarity results for the same set of sentences
- [ ] ⏱️ Measure processing time for each model
- [ ] 📝 Analysis: trade-off between speed and quality

**Expected result:** Practical knowledge of differences between models

---

### **Day 6: Visualization**
**Time:** 45-60 min  
**Objective:** Visualize embeddings in 2D for geometric intuition

**Activities:**
- [ ] 👨‍💻 Create `example_04_visualization.py`
- [ ] 📊 Use t-SNE or UMAP to reduce dimensionality
- [ ] 🎨 Plot embeddings with matplotlib/plotly
- [ ] 🏷️ Color points by categories (if applicable)
- [ ] 🔍 Interpret: do clusters make semantic sense?
- [ ] 📝 Capture screenshots of plots

**Expected result:** Visual intuition of how embeddings organize semantic information

---

### **Day 7: Final Mini-Project**
**Time:** 60-90 min  
**Objective:** Consolidate learning in practical project

**Activities:**
- [ ] 👨‍💻 Create `semantic_search_mini_project.py`
- [ ] 📚 Dataset: 20-30 sentences about various topics
- [ ] 🔍 Implement semantic search: given a query, return top-3 most similar
- [ ] 📊 Simple interface: user input → ranked results
- [ ] 🧪 Test with interesting queries
- [ ] 📝 Mini-project README with examples and results
- [ ] 🎉 Celebrate! Document general learnings from the week

**Expected result:** Functional semantic search application

---

## 📚 Study Resources

### **Essential Readings**
- [Embeddings — OpenAI](https://platform.openai.com/docs/guides/embeddings)
- [Sentence Transformers Documentation](https://www.sbert.net/)
- [The Illustrated Transformer](http://jalammar.github.io/illustrated-transformer/)

### **Complementary Readings**
- [HuggingFace Transformers Course](https://huggingface.co/learn/nlp-course/chapter1/1)
- [OpenAI Cookbook: Embeddings](https://github.com/openai/openai-cookbook/blob/main/examples/Getting_embeddings.ipynb)
- [Awesome Embeddings Papers](https://github.com/Separius/awesome-sentence-embedding)

### **Communities**
- [HuggingFace Discord](https://discord.gg/JfAtkvEtRb)
- [r/MachineLearning](https://reddit.com/r/MachineLearning)
- [OpenAI Community](https://community.openai.com/)

---

## 🛠️ Technical Setup

### **Dependencies**
```bash
# Add to requirements.txt
sentence-transformers==2.2.2
numpy==1.24.3
matplotlib==3.7.1
scikit-learn==1.3.0
umap-learn==0.5.3
plotly==5.15.0
pandas==2.0.3
```

### **File Structure**
```
week01-llms-embeddings/
├── notes.md                           # This file
├── experiments.md                     # Your notes
├── examples/
│   ├── example_01_basic.py
│   ├── example_02_similarity.py
│   ├── example_03_model_comparison.py
│   └── example_04_visualization.py
└── mini-project/
    ├── semantic_search_mini_project.py
    ├── example_dataset.txt
    └── README.md
```

---

## ✅ Learning Checklist

### **Theoretical Concepts**
- [ ] I can explain what LLMs are in 2 minutes
- [ ] I understand the difference between word vs sentence vs document embeddings
- [ ] I can explain cosine similarity and when to use it
- [ ] I know at least 3 practical applications of embeddings

### **Practical Skills**
- [ ] I can generate embeddings with Sentence Transformers
- [ ] I know how to calculate similarity between texts
- [ ] I tested at least 3 different models
- [ ] I created 2D visualization of embeddings
- [ ] I implemented basic semantic search

### **Final Project**
- [ ] Mini-project works correctly
- [ ] I documented code and results
- [ ] I identified limitations and next steps

---

## 📝 Space for Notes

### **Questions**
- (Note your questions here to research later)

### **Insights**
- (What surprised you most? What worked better/worse than expected?)

### **Project Ideas**
- (Ideas for future projects using embeddings) 