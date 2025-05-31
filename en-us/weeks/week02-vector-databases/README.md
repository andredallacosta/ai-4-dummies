# Week 2: Vector Databases in Practice

## 🎯 General Objective
Master the practical use of vector databases for efficient storage and semantic search, comparing different solutions and implementing production search systems.

---

## 📅 Daily Schedule (7 days)

### **Day 1: Vector Database Theory**
**Time:** 30-45 min  
**Objective:** Understand fundamental concepts and architectures of vector databases

**Activities:**
- [ ] 📖 Read: [What are Vector Databases?](https://www.pinecone.io/learn/vector-database/)
- [ ] 📖 Read: [Vector Databases Explained](https://weaviate.io/blog/what-is-a-vector-database)
- [ ] 📝 Map differences: vector database vs traditional database
- [ ] 🧠 List 5 use cases for vector databases
- [ ] 📝 Compare architectures: index-based vs graph-based

**Expected outcome:** Solid understanding of what vector databases are and when to use them

---

### **Day 2: ChromaDB Setup and Basics**
**Time:** 45-60 min  
**Objective:** Set up ChromaDB and perform first operations

**Activities:**
- [ ] ⚙️ Install ChromaDB: `pip install chromadb`
- [ ] 👨‍💻 Create `example_01_chromadb_basics.py`: first collection
- [ ] 🧪 Basic operations:
  - Create collection
  - Insert documents with embeddings
  - Similarity search
- [ ] 📊 Test with 10-20 simple documents
- [ ] 📝 Document configurations and behaviors

**Expected outcome:** ChromaDB working with basic operations

---

### **Day 3: Complete CRUD and Persistence**
**Time:** 45-60 min  
**Objective:** Implement all operations and data persistence

**Activities:**
- [ ] 👨‍💻 Create `example_02_complete_crud.py`
- [ ] 🔧 Implement:
  - Create: document insertion
  - Read: search and filtering
  - Update: document updates
  - Delete: document removal
- [ ] 💾 Set up local persistence
- [ ] 🧪 Test with larger dataset (100+ documents)
- [ ] 📝 Best practices for CRUD operations

**Expected outcome:** Complete and persistent CRUD system

---

### **Day 4: Optimization and Performance**
**Time:** 45-60 min  
**Objective:** Optimize queries and measure performance

**Activities:**
- [ ] 👨‍💻 Create `example_03_performance.py`
- [ ] 📊 Implement benchmarks:
  - Insertion time
  - Search latency
  - Query throughput
- [ ] 🔧 Test configurations:
  - Different embedding sizes
  - Various document numbers
  - Filters and metadata
- [ ] 📈 Analyze performance vs precision
- [ ] 📝 Optimization guide

**Expected outcome:** Optimized system with performance metrics

---

### **Day 5: Vector Database Comparison**
**Time:** 45-60 min  
**Objective:** Compare ChromaDB with other solutions

**Activities:**
- [ ] 👨‍💻 Create `example_04_comparison.py`
- [ ] 🧪 Implement search with:
  - ChromaDB (already implemented)
  - FAISS (Facebook AI Similarity Search)
  - Qdrant (if possible)
- [ ] 📊 Compare:
  - Ease of use
  - Performance
  - Available features
  - Scalability
- [ ] 📝 Detailed comparison matrix

**Expected outcome:** Complete comparative analysis of solutions

---

### **Day 6: Application Integration**
**Time:** 45-60 min  
**Objective:** Create REST API for vector database

**Activities:**
- [ ] 👨‍💻 Create `example_05_rest_api.py`
- [ ] 🌐 Implement FastAPI endpoints:
  - POST /documents (insert)
  - GET /search (search)
  - PUT /documents/{id} (update)
  - DELETE /documents/{id} (delete)
- [ ] 🧪 Test with Postman or curl
- [ ] 📊 Add metrics and logging
- [ ] 📝 API documentation with OpenAPI

**Expected outcome:** Working REST API for vector database

---

### **Day 7: Final Mini-Project**
**Time:** 60-90 min  
**Objective:** Complete semantic search system with web interface

**Activities:**
- [ ] 👨‍💻 Create `mini_semantic_search_project/`
- [ ] 🏗️ Implement complete system:
  - FastAPI backend with ChromaDB
  - Streamlit web interface
  - Document upload (PDF, TXT)
  - Real-time semantic search
- [ ] 📊 Advanced features:
  - Metadata filters
  - Search history
  - Relevance metrics
  - Result export
- [ ] 🧪 Test with real dataset (articles, documents)
- [ ] 📝 README with architecture and usage guide
- [ ] 🎉 Working end-to-end demo

**Expected outcome:** Production-ready semantic search system

---

## 📚 Study Resources

### **Essential Readings**
- [ChromaDB Documentation](https://docs.trychroma.com/)
- [Vector Databases Explained](https://www.pinecone.io/learn/vector-database/)
- [FAISS Documentation](https://faiss.ai/index.html)

### **Additional Readings**
- [Qdrant Documentation](https://qdrant.tech/documentation/)
- [Weaviate Concepts](https://weaviate.io/developers/weaviate/concepts)
- [Vector Search Algorithms](https://blog.research.google/2020/07/announcing-scann-efficient-vector.html)

### **Recommended Videos**
- [ChromaDB in 5 Minutes](https://www.youtube.com/watch?v=QdDoFfkVkcw)
- [Vector Databases Comparison](https://www.youtube.com/watch?v=klTvEwg3oJ4)

---

## 🛠️ Technical Setup

### **Dependencies**
```bash
# Add to requirements.txt
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

### **File Structure**
```
week02-vector-databases/
├── README.md                         # This file
├── experiments.md                    # Your notes
├── examples/
│   ├── example_01_chromadb_basics.py
│   ├── example_02_complete_crud.py
│   ├── example_03_performance.py
│   ├── example_04_comparison.py
│   └── example_05_rest_api.py
└── mini-project/
    ├── mini_semantic_search_project/
    │   ├── backend/
    │   │   ├── main.py               # FastAPI app
    │   │   ├── vector_db.py          # ChromaDB operations
    │   │   └── models.py             # Pydantic models
    │   ├── frontend/
    │   │   └── app.py                # Streamlit interface
    │   ├── data/                     # Test documents
    │   └── requirements.txt
    └── README.md
```

---

## ✅ Learning Checklist

### **Theoretical Concepts**
- [ ] I understand differences between vector and traditional databases
- [ ] I know the main vector search algorithms
- [ ] I know when to use each type of vector database
- [ ] I understand performance vs precision trade-offs

### **Practical Skills**
- [ ] I set up and used ChromaDB
- [ ] I implemented complete CRUD operations
- [ ] I optimized query performance
- [ ] I compared different solutions
- [ ] I created REST API for vector database

### **Final Project**
- [ ] Working semantic search system
- [ ] Intuitive web interface
- [ ] Documented API
- [ ] Optimized performance
- [ ] Complete documentation

---

## 📝 Space for Notes

### **Solution Comparison**
- **ChromaDB:**
  - Pros:
  - Cons:
  - Best for:

- **FAISS:**
  - Pros:
  - Cons:
  - Best for:

### **Performance Metrics**
- Insertion time:
- Search latency:
- Result precision:
- Memory usage:

### **Optimal Configurations**
- Embedding size:
- Search algorithm:
- Index parameters:

### **Problems Encountered**
- (Technical difficulties and solutions)

### **Ideas for Next Projects**
- (Practical applications with vector databases) 