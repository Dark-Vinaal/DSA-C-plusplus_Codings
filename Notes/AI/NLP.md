## 🗣️ Natural Language Processing (NLP)

- **Natural Language Processing (NLP)** is the field of AI that enables computers to understand, interpret, and generate human language. In 2025, NLP has moved beyond simple word-matching to deep semantic understanding.

---

### 1. The Core NLP Pipeline

Before a model can "understand" a sentence, it must break it down using several linguistic processing steps:
 
* **Tokenization:** The process of breaking text into smaller units called **tokens** (words, subwords, or characters).
* **Part-of-Speech (POS) Tagging:** Assigning grammatical labels to each token (e.g., Identifying "Apple" as a *Noun* and "is" as a *Verb*).
* **Named Entity Recognition (NER):** Detecting and classifying "entities" in text such as **People**, **Places**, **Organizations**, or **Dates**.
* **Lemmatization:** Reducing words to their base or dictionary form (e.g., "running" → "run").

---

### 2. From Words to Math: Vectors & Embeddings

Computers cannot process words; they process numbers.

* **Vector/Embedding:** A mathematical representation of a word or sentence in a high-dimensional space. Words with similar meanings (e.g., "King" and "Queen") are placed close together in this **Vector Space**.
* **Dimensionality:** Modern embeddings can have 768, 1536, or more dimensions, each representing a hidden feature of the word's meaning.



---

### 3. Storing Knowledge: Vector Databases

Traditional databases (SQL) search for exact matches. **Vector Databases** search for **meaning**.
* **Definition:** A specialized database (e.g., **Pinecone**, **Milvus**, **Weaviate**) designed to store and index high-dimensional vectors.
* **Similarity Search:** Uses algorithms like **HNSW** (Hierarchical Navigable Small World) and **Cosine Similarity** to find the "nearest neighbors" to a query vector.
* **Use Case:** This is the backbone of **RAG (Retrieval-Augmented Generation)**, allowing AI to look up your private documents to answer questions.

---

### 4. Model Optimization & Specialization

- How do we make a general AI an expert in a specific field?

#### **A. Specialization (Domain Adaptation)**

Using models pre-trained on specific data types.
* **BioBERT:** Specialized for medical/biological text.
* **LegalBERT:** Specialized for legal documents and contracts.

#### **B. Fine-Tuning**

The process of taking a pre-trained model and "tweaking" its weights on a smaller, specific dataset.
* **Full Fine-Tuning:** Updating all parameters (expensive/heavy).
* **PEFT (Parameter-Efficient Fine-Tuning):** Updating only a tiny fraction of the model. 
    * **LoRA (Low-Rank Adaptation):** The 2025 industry standard. It adds small "plug-in" layers to the model, making it 10,000x more efficient to train.

---

### 5. NLP vs. LLM: What’s the difference?

* **Traditional NLP:** Focused on specific tasks like "Is this email spam?" or "Is this review positive?" (Classification).
* **Modern LLMs:** Use the foundations of NLP to **generate** coherent, human-like text across any domain (Generative).

---
