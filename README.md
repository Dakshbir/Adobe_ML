# AI-Powered SQL Query Generation and Correction Agent

## 🚀 Overview
This project provides an AI-driven backend service capable of:
- Generating accurate SQL queries from natural language inputs.
- Automatically correcting erroneous SQL queries (syntax errors, incorrect attributes, or tables).

The solution leverages advanced NLP techniques, schema-aware query generation, and query correction methods to simplify database interactions for technical and non-technical users.

---

## 🛠 Tech Stack Used

| Technology / Tool                | Purpose / Role                                      |
|----------------------------------|-----------------------------------------------------|
| *Python (3.7+)*                | Core programming language                           |
| *PostgreSQL*                   | Database management                                 |
| *Groq API (LLama2-7b)*         | Large Language Model (LLM) for NLP tasks            |
| *Flask*                        | Backend API framework                               |
| *psycopg2-binary*              | PostgreSQL database connection                      |
| *python-dotenv*                | Secure environment variable management              |
| *Groq Python SDK*              | Official SDK for Groq API integration               |

---

## 🎯 Approach Used

### 1. Natural Language to SQL Query Generation
- Leveraged Groq's LLama2-7b model to interpret user intent.
- Integrated dynamic database schema extraction to ensure accuracy.
- Implemented few-shot learning prompts using provided training datasets.

### 2. SQL Query Correction
- Used Groq's LLama2-7b model trained on provided correction examples.
- Dynamically provided schema context to ensure corrected queries align with the database.
- Included robust retry mechanisms and error handling to ensure reliability.

---

## 📂 Project Structure
