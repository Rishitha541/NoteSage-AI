# 📘 NoteSage – AI

NoteSage – AI is an **AI-powered web application** that transforms static study materials into interactive learning aids.  
It helps students by generating **summaries, mind maps, and Q&A** from uploaded notes, making self-study faster and more engaging.

---

## 🔎 How It Works

### 1. Input Layer – Upload Notes
- Users upload study materials (PDFs, PPTs, text files).
- The system extracts raw text using parsing libraries.
- Preprocessing cleans the text (removes formatting, tokenizes, and organizes content).

### 2. AI Processing Pipeline
- **Summarization:** Condenses large notes into concise summaries using NLP models.  
- **Mind Map Generation:** Identifies key concepts and relationships, then structures them into a graph/tree visualization.  
- **Q&A System:** Uses semantic search + embeddings to find relevant sections in notes and generate answers.  
- **Simplified Explanations:** Breaks down complex terms with analogies and real-world examples.

### 3. Backend – FastAPI
- Handles file uploads, API calls, and database queries.
- Connects the frontend with AI models (e.g., GPT-based services).
- Stores metadata about uploaded notes and user sessions.

### 4. Frontend – React
- Provides an interactive dashboard for students.
- Features:
  - Upload panel for study materials
  - Summaries and mind maps display
  - Real-time Q&A interface
- Built with **React + TypeScript** for a clean, responsive UI.

---

## 🔄 Continuous Data Flow


- **Step 1:** User uploads notes → text is extracted and cleaned.  
- **Step 2:** AI models generate summaries, mind maps, and answers.  
- **Step 3:** Backend manages requests, stores metadata, and connects AI services.  
- **Step 4:** Frontend displays results in a user-friendly interface.  
- **Step 5:** User continues interacting (asking questions, requesting new summaries).  

This cycle repeats continuously, making study materials dynamic and interactive.

---

## 🛠️ Tech Stack
- **Languages:** HTML, CSS, JavaScript, TypeScript, SQL  
- **Frameworks/Tools:** React, FastAPI  
- **AI Tools:** ChatGPT, NLP models, embeddings  
- **Other Tools:** VS Code, GitHub, Replit  

---

## 🎯 Why It’s Useful
- Saves time by condensing large notes into digestible chunks.  
- Helps visualize relationships between concepts.  
- Provides instant clarification of doubts.  
- Makes self-study more interactive and personalized.  

---
