# Week 3: Retrieval-Augmented Generation (RAG)

## 🎯 General Objective
Master the concept and practical implementation of RAG (Retrieval-Augmented Generation), combining semantic search with text generation to create intelligent Q&A systems.

---

## 📅 Daily Schedule (7 days)

### **Day 1: RAG Theory and Architecture**
**Time:** 30-45 min  
**Objective:** Fully understand the concept of RAG and its architecture

**Activities:**
- [ ] 📖 Read: [What is RAG?](https://blogs.nvidia.com/blog/2023/11/13/what-is-retrieval-augmented-generation/)
- [ ] 📖 Read: [RAG vs Fine Tuning](https://www.pinecone.io/learn/retrieval-augmented-generation/)
- [ ] 📝 Draw RAG architecture diagram (Retrieval → Augmentation → Generation)
- [ ] 🧠 List 5 use cases where RAG is better than fine-tuning
- [ ] 📝 Summarize RAG advantages and limitations

**Expected outcome:** Solid understanding of what RAG is and when to use it

---

### **Day 2: LangChain Fundamentals**
**Time:** 45-60 min  
**Objective:** Setup and first steps with LangChain for RAG

**Activities:**
- [ ] 📖 Read: [LangChain RAG Tutorial](https://python.langchain.com/docs/use_cases/question_answering/)
- [ ] ⚙️ Install dependencies: langchain, openai, chromadb
- [ ] 👨‍💻 Create `example_01_langchain_basics.py`: loader + splitter + embeddings
- [ ] 🧪 Test with simple text document (PDF or TXT)
- [ ] 📝 Document each component: DocumentLoader, TextSplitter, VectorStore

**Expected outcome:** Basic document ingesting pipeline working

---

### **Day 3: LlamaIndex Fundamentals**
**Time:** 45-60 min  
**Objective:** Compare LlamaIndex approach vs LangChain

**Activities:**
- [ ] 📖 Read: [LlamaIndex Quickstart](https://docs.llamaindex.ai/en/stable/getting_started/starter_example.html)
- [ ] ⚙️ Install llama-index
- [ ] 👨‍💻 Create `example_02_llamaindex_basics.py`: SimpleDirectoryReader + VectorStoreIndex
- [ ] 🧪 Use same document from previous day
- [ ] 📊 Compare: ease of use, speed, response quality
- [ ] 📝 Document differences between LangChain and LlamaIndex

**Expected outcome:** Mastery of two main frameworks for RAG

---

### **Day 4: Chunking Strategies**
**Time:** 45-60 min  
**Objective:** Optimize text splitting strategies for better retrieval

**Activities:**
- [ ] 👨‍💻 Create `example_03_chunking_strategies.py`
- [ ] 🧪 Test different approaches:
  - Character splitting (fixed size)
  - Recursive character splitting
  - Semantic chunking
  - Document-aware splitting
- [ ] 📊 Compare response quality for each method
- [ ] 🔍 Analyze: which chunking works best for which document type?
- [ ] 📝 Document chunking best practices

**Expected outcome:** Expertise in chunking optimization for different scenarios

---

### **Day 5: Prompt Engineering for RAG**
**Time:** 45-60 min  
**Objective:** Improve response quality through prompt engineering

**Activities:**
- [ ] 👨‍💻 Create `example_04_prompt_engineering.py`
- [ ] 🧪 Test different prompt templates:
  - Basic: "Answer based on context: {context}\nQuestion: {question}"
  - Detailed: Specific instructions on how to respond
  - Chain-of-thought: Ask to explain reasoning
  - Few-shot: Include examples
- [ ] 📊 Evaluate response quality for each template
- [ ] 🔍 Identify when each prompt type works best
- [ ] 📝 Create reusable prompt library

**Expected outcome:** Library of optimized prompts for different use cases

---

### **Day 6: Evaluation and Metrics**
**Time:** 45-60 min  
**Objective:** Implement metrics to evaluate RAG system quality

**Activities:**
- [ ] 👨‍💻 Create `example_05_evaluation.py`
- [ ] 📊 Implement metrics:
  - Relevance of retrieved documents
  - Response quality (BLEU, ROUGE if possible)
  - Response time
- [ ] 🧪 Create test dataset with questions and expected answers
- [ ] 📈 Compare performance of different configurations
- [ ] 📝 Simple dashboard to visualize metrics

**Expected outcome:** Automated RAG evaluation system

---

### **Day 7: Final Mini-Project**
**Time:** 60-90 min  
**Objective:** Complete Q&A system over personal documents

**Activities:**
- [ ] 👨‍💻 Create `mini_personal_qa_project.py`
- [ ] 📚 Dataset: Personal documents (PDFs, saved articles, notes)
- [ ] 🏗️ Complete pipeline: ingestion → chunking → embedding → retrieval → generation
- [ ] 💻 Interface: Streamlit or gradio for interaction
- [ ] 🧪 Test with complex questions about your documents
- [ ] 📊 Include real-time evaluation metrics
- [ ] 📝 Detailed README with architecture and results
- [ ] 🎉 Working demo + limitations analysis

**Expected outcome:** Complete and functional RAG system for personal use

---

## 📚 Study Resources

### **Essential Readings**
- [RAG with LlamaIndex](https://docs.llamaindex.ai/en/stable/getting_started/concepts.html)
- [RAG with LangChain](https://python.langchain.com/docs/use_cases/question_answering/)
- [Chunking Strategies](https://www.pinecone.io/learn/chunking-strategies/)

### **Additional Readings**
- [Advanced RAG Techniques](https://blog.langchain.dev/semi-structured-multi-modal-rag/)
- [RAG vs Fine-tuning](https://www.anyscale.com/blog/a-comprehensive-guide-for-building-rag-based-llm-applications-part-1)
- [Evaluation of RAG Systems](https://blog.langchain.dev/evaluating-rag-pipelines-with-ragas-langsmith/)

### **Recommended Videos**
- [LangChain RAG from Scratch](https://www.youtube.com/watch?v=LhnCsygAvzY)
- [LlamaIndex in 5 Minutes](https://www.youtube.com/watch?v=hA1JPOy9KCc)

---

## 🛠️ Technical Setup

### **Dependencies**
```bash
# Add to requirements.txt
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

### **File Structure**
```
week03-rag/
├── notes.md                          # This file
├── experiments.md                    # Your notes
├── examples/
│   ├── example_01_langchain_basics.py
│   ├── example_02_llamaindex_basics.py
│   ├── example_03_chunking_strategies.py
│   ├── example_04_prompt_engineering.py
│   └── example_05_evaluation.py
└── mini-project/
    ├── mini_personal_qa_project.py
    ├── streamlit_interface.py
    ├── documents/                    # Your test documents
    ├── prompts_library.py
    └── README.md
```

---

## ✅ Learning Checklist

### **Theoretical Concepts**
- [ ] I can explain RAG vs fine-tuning in 3 minutes
- [ ] I understand the components: Retrieval, Augmentation, Generation
- [ ] I know when to use LangChain vs LlamaIndex
- [ ] I know different chunking strategies

### **Practical Skills**
- [ ] I implemented RAG with LangChain
- [ ] I implemented RAG with LlamaIndex
- [ ] I tested different chunking strategies
- [ ] I created optimized prompts for RAG
- [ ] I implemented evaluation system

### **Final Project**
- [ ] Q&A system working with personal documents
- [ ] Web interface for interaction
- [ ] Evaluation metrics implemented
- [ ] Complete documentation

---

## 📝 Space for Notes

### **LangChain vs LlamaIndex Comparison**
- **LangChain:**
  - Pros:
  - Cons:
- **LlamaIndex:**
  - Pros:
  - Cons:

### **Best Chunking Strategies**
- For technical documents:
- For narratives/books:
- For academic articles:

### **Prompts That Worked Well**
- (Paste here the prompts that gave the best results)

### **Identified Limitations**
- (What didn't work well? What problems did you encounter?)

### **Ideas for Next Projects**
- (Inspirations for more advanced projects with RAG) 