**Ask Data – Retrieval-Augmented Generation (RAG) 📂🤖

Ask Data is a Retrieval-Augmented Generation (RAG) project that lets you query your documents and datasets in plain English. 
Instead of manually searching PDFs or writing SQL, you can just ask a question, and the system retrieves relevant information and generates a clear answer using a Large Language Model (LLM).

⸻

✨ Features
	•	🔍 RAG-powered Q&A – Combines retrieval + generation for accurate answers.
	•	📑 Document Understanding – Splits documents into chunks and retrieves only the relevant sections.
	•	🧠 Conversational Memory – Supports follow-up questions with context retention.
	•	⚡ Fast Vector Search – Embeddings stored in a vector DB for quick lookups.
	•	🖥️ Notebook Interface – Built in Jupyter for experimentation and learning.

⸻

🛠️ Tech Stack
	•	Python – Core language
	•	LangChain – Orchestrates RAG pipeline (retriever + LLM)
	•	Groq API – LLaMA 70B – LLM for response generation
	•	ChromaDB – Vector database for document embeddings
	•	SentenceTransformers – Creates embeddings for semantic similarity
	•	PyPDF / NumPy / Pandas – Data handling utilities

⸻

⚙️ RAG Workflow
	1.	Data Ingestion
	•	Load documents (e.g., PDF, text).
	•	Split into smaller chunks for embedding.
	2.	Embedding Creation
	•	Convert each chunk into numerical vectors using SentenceTransformers.
	3.	Vector Store
	•	Store embeddings in ChromaDB for similarity search.
	4.	Query & Retrieval
	•	User enters a question → converted into an embedding.
	•	Retriever searches for the most relevant chunks.
	5.	Generation
	•	Retrieved chunks are passed to LLaMA 70B via Groq API.
	•	The LLM generates a contextual, human-like answer.
