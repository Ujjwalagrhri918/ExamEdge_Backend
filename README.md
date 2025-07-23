# ExamEdge_Backend

The backend of ExamEdge, an AI-powered study assistant that processes PDF-based study material to generate summaries, quizzes, and helpful resources for students.

🚀 Features (Backend Focus)
📄 PDF Text Extraction

Uses PyMuPDF (fitz) to extract structured text from uploaded PDFs.

Falls back to OCR using pytesseract if the PDF contains scanned images.

🧠 AI Summarization via Gemini

Integrates with Google Gemini Pro to summarize extracted content into digestible, student-friendly notes.

Extracts key points and insights for focused revision.

❓ MCQ Generation

Dynamically generates multiple-choice questions based on PDF content using Gemini prompts.

🎥📚 Supplementary Resource Suggestions

Recommends relevant videos (e.g., YouTube) and books aligned with the uploaded content.

💬 Interactive AI Chat

Supports natural language queries via Gemini for deeper understanding or clarification.

👩‍🏫 Expert Connect Integration

Backend endpoint for scheduling sessions with subject matter experts.


🛠️ Tech Stack
FastAPI – Lightweight and async Python framework to serve all backend endpoints.

Ngrok – Used to expose the local FastAPI server to the internet for frontend integration and testing.

PyMuPDF (fitz) – PDF parsing and text extraction.

pytesseract – OCR engine for image-based text.

google-generativeai – Connects to Gemini API for summarization and content generation.

