# TicketMind
<img width="1919" height="943" alt="Screenshot 2026-01-03 000530" src="https://github.com/user-attachments/assets/06e00a86-7475-446e-94d1-a06e68f7e8d4" />
User / Client
     |
     v
+----------------------+
| Incoming Ticket      |
| (Subject + Body)     |
+----------------------+
     |
     v
+----------------------+
| Text Preprocessing   |
| - Clean text         |
| - Lowercasing        |
| - Tokenization       |
+----------------------+
     |
     v
+----------------------------------+
| Feature Extraction (TF-IDF)      |
| - Subject Vectorizer             |
| - Body Vectorizer                |
+----------------------------------+
     |
     v
+----------------------------------+
| Multi-Label ML Classifier        |
| - Predict Type                  |
| - Predict Queue                 |
| - Predict Priority              |
| - Confidence Scores             |
+----------------------------------+
     |
     v
+----------------------------------+
| Initial Label Prediction         |
| {Type, Queue, Priority}          |
+----------------------------------+
     |
     v
+----------------------------------+
| Semantic Embedding (Sentence-BERT|
| / Gemini Embeddings)             |
+----------------------------------+
     |
     v
+----------------------------------+
| Vector Database (FAISS)          |
| - Retrieve Top-K Similar Tickets |
+----------------------------------+
     |
     v
+----------------------------------+
| RAG Validation Layer             |
| - Majority voting from history   |
| - Agreement threshold check      |
| - Correct ML predictions if needed|
+----------------------------------+
     |
     v
+----------------------------------+
| Final Validated Labels           |
| {Type, Queue, Priority}          |
+----------------------------------+
     |
     v
+----------------------------------+
| Context Construction             |
| - Previous resolutions           |
| - Similar ticket answers         |
+----------------------------------+
     |
     v
+----------------------------------+
| LLM (Gemini)                     |
| - Prompt with ticket + context   |
| - Generate human-like response   |
+----------------------------------+
  


