AI-Assisted Student Doubt Resolution with Faculty Resource and Analytics Platform
📌 Overview
This project is a full-stack academic support platform that enables structured doubt resolution and faculty-driven resource management.
The system allows students to ask academic doubts, tracks repeated questions for analytics, and provides AI-generated conceptual explanations. Faculty can upload verified study materials and analyze frequently asked doubts through an Insight Hub.
🚀 Features
Student doubt submission and tracking
Automatic askedCount increment for repeated doubts
AI-generated conceptual explanations (via locally hosted LLM using Ollama)
Faculty-verified resource upload (PDF-based)
Insight Hub analytics for identifying weak academic topics
RESTful API-based frontend–backend communication
🛠️ Tech Stack
Frontend
HTML
CSS
JavaScript (Fetch API)
Backend
Java
Spring Boot
REST APIs
Database
MySQL
AI Integration
Ollama (Locally hosted LLM model such as Mistral/LLaMA)
🧠 System Workflow
Student submits a doubt.
Backend checks if the doubt exists:
If yes → increments askedCount.
If no → stores doubt and sends it to the AI model.
AI generates a short conceptual explanation.
Faculty can view analytics in the Insight Hub.
Faculty upload verified study resources accessible to students.
📂 Project Modules
1️⃣ Student Module
Ask doubts
View AI responses
Explore faculty-uploaded resources
2️⃣ Faculty Module
Upload verified PDFs
View analytics table of frequently asked doubts
3️⃣ Insight Hub
Displays doubt frequency analytics
Helps identify commonly misunderstood topics
📦 File Upload Handling
Uses Spring Boot MultipartFile
Stores PDFs in /uploads directory
Metadata saved in MySQL
Files served through REST endpoint
🔐 Security & Validation
File type validation (PDF only)
Backend request validation
CORS configuration enabled for frontend communication
📈 Future Enhancements
Role-based authentication (Student/Faculty login)
Graphical analytics dashboard
Cloud deployment (AWS/Azure)
Advanced AI model tuning
👨‍💻 Author
Aligeti Shalini
