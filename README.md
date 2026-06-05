######################
# SmartHire AI Agent #
######################

## 📌 Project Overview
SmartHire AI Agent is a text-based AI Mock Interview System that conducts technical interviews, evaluates answers using a locally running LLM (Llama3 via Ollama), and generates a detailed performance report.

The system helps students practice interviews and get AI-powered feedback including scoring, improvements, and suggestions.

---

## 🎯 Main Objective
The main goal of this project is to help students prepare for technical interviews using an AI-driven system.

It helps learners understand:
- Generative AI
- AI Agents
- Large Language Models (LLMs)
- Prompt Engineering
- Interview Automation
- Answer Evaluation Systems
- Report Generation
- Memory-based AI workflows

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|--------|
| Python | Core programming language |
| Ollama | Runs local LLM server |
| Llama3 | AI model for evaluation |
| requests | API communication with Ollama |
| os | File and folder handling |
| datetime | Timestamp generation |

---

## 📁 Project Structure

SmartHire_AI_Agent/
│
├── main.py                 # Entry point of the application
├── interview_agent.py     # Core AI agent logic
├── llm_engine.py          # LLM (Ollama) API integration
├── questions.py           # Question bank
├── report_generator.py    # Generates final report
│
└── reports/               # Stores generated interview reports

---

## ⚙️ File Explanation

### 1. main.py
This is the entry point of the project. It:
- Displays project header
- Accepts student name
- Shows interview menu
- Starts full or topic-wise interview
- Controls overall flow

---

### 2. questions.py
Contains the question bank used in interviews.

Topics include:
- Python
- OOP
- Machine Learning
- Deep Learning
- Transformers
- LLM
- RAG
- AI Agents

Example:
{
  "topic": "Python",
  "question": "Explain the difference between list, tuple and set in Python."
}

---

### 3. interview_agent.py
Core AI engine of the system:
- Builds prompts for LLM
- Sends answers for evaluation
- Extracts score
- Maintains interview history
- Generates final report

Key Methods:
- evaluate_answer()
- extract_score()
- generate_final_report()

---

### 4. llm_engine.py
Connects Python with Ollama (Llama3 model).

Endpoint:
http://localhost:11434/api/generate

Payload:
{
  "model": "llama3",
  "prompt": prompt,
  "stream": false
}

---

### 5. report_generator.py
Saves final interview report:
- Creates reports folder
- Adds timestamp
- Saves .txt file

---

## 🔄 Project Flow

User starts program
↓
main.py executes
↓
Student enters name
↓
Interview mode selected
↓
Questions loaded
↓
Student answers
↓
LLM evaluates answer
↓
Score generated
↓
History stored
↓
Final report created
↓
Saved in reports folder

---

## 🧠 AI Agent Concepts

Input: Student answer  
Brain: Llama3  
Tool: Ollama API  
Memory: Interview history  
Output: Evaluation + Report  

---

## 🚀 Features
- AI mock interviews
- Topic-wise questions
- Real-time evaluation
- Score generation
- Feedback system
- Report generation
- Local LLM integration


## Authon

#######################
- Parag Kiran Udgirkar 
#######################
