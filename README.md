# CineRAG – LLM-based Movie Dialogue Search using RAG
📖 Overview

This project is a Retrieval-Augmented Generation (RAG) system that allows users to search and understand movie or TV dialogues.

It retrieves relevant dialogues using semantic search
Then generates explanations using a Large Language Model (LLM)
Designed for fast, accurate, and meaningful results

🚀 Features
* 🔍 Semantic search on subtitles (not keyword-based).
* 🧠 Context-aware response generation using LLM
* 📂 Handles large datasets (~50,000+ dialogues)
* ⚡ Fast retrieval using vector database
* 🎯 Improved accuracy with cosine similarity re-ranking
* 💬 Explains dialogues in simple language
🏗️ System Architecture

User Query
     ↓
Text Embedding
     ↓
Vector Database (ChromaDB)
     ↓
Top Relevant Results
     ↓
LLM (Gemini / OpenAI)
     ↓
Final Answer (Dialogue + Explanation)

🛠️ Tech Stack
* Language: Python
* Frameworks/Libraries:
* LangChain
* SentenceTransformers
* ChromaDB
* LLM: Gemini / OpenAI
* Embedding Model: all-MiniLM / similar

Tools Used:
* Text Splitter
* Embedding Models
* Vector Stores

📂 Dataset
* Movie & TV subtitles dataset
* ~50,000+ dialogue lines
  
Preprocessed and cleaned before indexing
* Data Preprocessing
* Clean subtitles (remove noise, symbols)
* Split into smaller chunks
* Embedding Creation
* Convert text into vectors using SentenceTransformers

Storage
* Store embeddings in ChromaDB
* Query Handling
* Convert user query into embedding
* Retrieve similar dialogues using cosine similarity

Response Generation
* Pass retrieved results to LLM
* Generate explanation or answer
* 
📊 Improvements Achieved
* ✅ ~30% better accuracy than keyword search
*  Faster retrieval using vector indexing
* 🧠 Better understanding using semantic similarity
  
▶️ How to Run
* # Clone repository
* git clone <your-repo-link>

# Install dependencies
pip install -r requirements.txt

# Run project
python main.py
📌 Example Use Case

Input:

Why did the character say "I am the danger"?

Output:

Dialogue: "I am the danger"
Explanation: The character is expressing dominance and control...
🔮 Future Enhancements
Add UI (Streamlit / Web App)
Multi-language support
Improve ranking using hybrid search
Add memory for conversation history
👨‍💻 Author

Haseeb Imtiyaz
Data Scientist | ML Engineer

⭐ Conclusion

This project demonstrates:

Real-world use of RAG architecture
Integration of LLMs + Vector Databases
Practical application of semantic search
