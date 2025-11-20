Placenix — AI Driven Placement Assistant

This project introduces Placenix, an AI-powered Placement Management Assistant built using FastAPI + OpenAI + ChromaDB + React/Tailwind.
It supports smart Q/A, resume analysis, RAG-based custom data retrieval, streaming chat, and placement prediction.

 Project Highlights

 AI Chatbot using OpenAI GPT models

 Resume analyzer (PDF based)

 RAG search using Chroma Vector DB

 Real-time streaming chat

 Placement prediction using ML model

 Backend built with FastAPI, Frontend with React/Tailwind

 Features
1. AI Chat (General Queries)

Ask anything about placements, companies, skills, resume tips.

2. RAG Chat (College / Company Specific Info)

Uses ChromaDB vector search

Retrieve custom placement rules, criteria, TPO data

3. Resume Analyzer

Upload PDF resume → AI gives structured feedback

Skills, mistakes, improvements

4. Placement Predictor

Predict placement probability based on:

CGPA

Backlogs

Internships

Projects

5. Streaming Chat

ChatGPT-like typing effect using Server-Sent Events

 Visual Overview

(Add your own images later — I’m leaving placeholders)

 1. System Architecture Diagram
<Add Image Here>

 2. Chat UI Screenshot
<Add Image Here>

 3. API Response Examples
<Add Image Here>

 Tech Stack

 Python (FastAPI)

 OpenAI GPT

 ChromaDB Vector Database

 React + Tailwind CSS

 Uvicorn Server

 Repository Structure
Placenix/
│
├── backend/
│   ├── app/
│   ├── main.py
│   ├── requirements.txt
│   └── .env   (excluded)
│
└── frontend/
    ├── src/
    ├── index.html or React App
    └── tailwind.config.js

Backend Setup
Create .env file
OPENAI_API_KEY=your_key_here
CHROMA_DIR=./chroma_db

 Install dependencies
pip install -r requirements.txt

 Run FastAPI Server
uvicorn app.main:app --reload --port 8000

API docs available at:

http://localhost:8000/docs

API Endpoints
POST /api/chat

General AI chat

GET /stream-chat

Real-time typing response

POST /api/ingest

Add documents to Vector DB

POST /api/rag-chat

Chat using your custom placement data

POST /api/resume/analyze

Upload a resume (PDF)

 POST /api/predict

Placement probability prediction

Frontend Setup
npm install
npm start


Frontend runs at:
 http://localhost:3000/

Learnings

How to integrate LLMs with FastAPI

Implementing RAG pipelines

Using ChromaDB for vector search

Building a complete ML + AI system

Designing a chatbot UI with streaming

Future Enhancements

Add admin dashboard

Student performance analytics

Integration with WhatsApp bot

Deploy on Render/EC2

Add authentication system

