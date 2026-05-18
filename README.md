# 1. Applied Prompt Engineering: Prompt Testing and Evaluation with Promptfoo

<p align="center">
  <img src="https://github.com/user-attachments/assets/63838e5d-417b-4b34-94c1-486c3d80f222" width="23%" />
  <img src="https://github.com/user-attachments/assets/dc6894b7-6fcb-460a-b120-2933b1ab0952" width="23%" />
  <img src="https://github.com/user-attachments/assets/52a9d432-2b57-4b14-9609-554ff1f02b64" width="23%" />
  <img src="https://github.com/user-attachments/assets/36abc6f0-797b-468b-aada-ec42b55c003a" width="23%" />
</p>

## What I Have Done
In this project, I explored and evaluated different prompt engineering techniques using Promptfoo. I designed and tested four types of prompts:

1. Standard Prompt  
2. Emotional Stimuli Prompt  
3. Expert Persona Prompt  
4. Zero-shot Chain-of-Thought (CoT) Prompt  

The evaluation was conducted using the OpenAI model (`gpt-4o-mini`) as both the response generator and LLM judge. I used a dataset of structured questions (MMLU Astronomy) stored in a Google Sheet and integrated it into Promptfoo for automated testing.

The experiment included:
- Running prompt evaluations across multiple test cases  
- Comparing prompt performance using pass/fail metrics  
- Using an LLM-based judge for semantic evaluation  
- Tracking token usage, cost, and execution time  

In total, I ran 1824 individual test cases including evaluation by an LLM judge.

---
## Why It Is Important

Prompt engineering plays a critical role in improving the quality and reliability of LLM outputs. This project demonstrates:

- How different prompt strategies impact model performance  
- The importance of structured evaluation instead of intuition  
- The use of LLM-as-a-judge for semantic correctness  
- Trade-offs between cost, latency, and accuracy when scaling across models  

Additionally, testing across multiple models significantly increases both cost and runtime. For example:

- Total duration (3 models): ~37 minutes  
- Total tokens: >1 million  
- Total cost: ~$3.34  

Breakdown:
- OpenAI: $0.15  
- Claude Sonnet: $2.96  
- Gemini: $0.00 (free tier)  

This highlights the importance of efficient evaluation strategies in real-world AI systems.

---

## Technologies Used

- Promptfoo (prompt evaluation framework)  
- OpenAI API (`gpt-4o-mini`)  
- Anthropic Claude (Sonnet)  
- Google Gemini  
- Google Sheets (test dataset)  
- Node.js (Promptfoo runtime)  
- Python (environment setup and utilities)  

---

## Key Takeaways

- Prompt design significantly affects output quality  
- Emotional and role-based prompts can improve responses in some cases  
- Chain-of-Thought prompting helps with reasoning tasks  
- Automated evaluation pipelines are essential for scalable prompt engineering  
- Cost and token usage must be carefully managed when testing multiple models
_____________________________________________________________________________________________________________________________________________________
# 2. AI Automation

#  Project Overview  AI Document Q&A Agent (n8n)

<p align="center">
  <img src="https://github.com/user-attachments/assets/04e3f96b-8a85-46f9-98f1-e26d8d4d453a" width="300" />
  <img src="https://github.com/user-attachments/assets/008033d4-9564-4320-be20-11cc44a90a8f" width="300" />
  <img src="https://github.com/user-attachments/assets/a3e96b88-0e91-4226-a72f-2e8f4056303c" width="300" />
</p>

This project is an AI-powered RAG (Retrieval-Augmented Generation) system built in n8n.
It allows you to upload a PDF document to Google Drive and ask questions about its content.
The workflow retrieves relevant text from the document using a vector database and generates accurate answers with OpenAI GPT-4o-mini.

📌How This Project Helps People and Organizations

This AI Document Q&A Agent can be extremely useful for anyone who works with large documents, manuals, reports, or internal files.
Instead of searching manually through long PDFs, users can simply ask questions and get accurate answers instantly.

📌Who Can Benefit

- Students & Researchers — quickly extract important information from academic papers

- Teams & Organizations — make internal documents searchable and interactive

- Customer Support — turn product manuals into smart, conversational knowledge bases

- Managers & Executives — access key insights from long reports without reading everything

- Educators — create instant Q&A systems for course materials

- Engineers / Developers — build custom chatbots for private documents

📌How It Helps

- Instant Information Retrieval
No need to scroll through a PDF — ask a question and get the exact answer.

- Automated Knowledge Extraction
Converts any document into a searchable knowledge base using AI.

- Context-Aware Answers
Uses the uploaded document as the only source, ensuring grounded and accurate responses.

- Saves Time
Reduces hours of manual reading, searching, and summarizing.

- Private & Secure
Your data stays inside your own n8n workflow and vector database.

- Increases Productivity
Teams can make faster decisions by retrieving essential information instantly.

📌Key Steps:

- Load a PDF file stored in Google Drive

- Split the document into text chunks

- Convert chunks into embeddings using OpenAI

- Store embeddings in a Pinecone vector database

- Retrieve the most relevant chunks based on user queries

- Generate context-aware answers using GPT-4o-mini

- Interact with the agent using n8n’s built-in chat interface

📌Output

- Accurate answers grounded in the uploaded PDF

- Fast, semantic search over document content

- Fully automated workflow for document processing

- Real-time Q&A capability through n8n


_____________________________________________________________________________________________________________________________________________________

# 3. 🤖 AI Assistant for PhD Program Information (RAG-based Chatbot)
### [👉Click here to view the Live App](https://llms-phd-program.streamlit.app/)

<p align="center">
  <img src="https://github.com/user-attachments/assets/e35eed80-8a84-4225-b60b-928e3d78a49a" />
</p>

## What I Have Done

I developed a Retrieval-Augmented Generation (RAG) chatbot application that allows users to interact with and query information from documents, specifically focused on PhD program details.

The system processes PDF documents, extracts and chunks the text, converts it into vector embeddings using OpenAI models, and stores them in a Pinecone vector database. When a user asks a question, the system retrieves the most relevant information from the database and generates a response using a language model.

This approach enables accurate, context-aware answers instead of generic responses.

### Business Value

This solution can be applied across multiple business domains:

- **Knowledge Management**: Enables organizations to query internal documents (policies, manuals, reports) efficiently.
- **Customer Support Automation**: Provides instant, context-aware answers based on company documentation.
- **Education & Training**: Helps users explore structured content such as academic programs or training materials.
- **Decision Support Systems**: Allows quick access to relevant insights from large datasets.

Overall, it reduces manual effort, improves information accessibility, and enhances user experience.
---

## Technologies Used

- **Python**
- **Streamlit** (UI and deployment)
- **OpenAI API** (embeddings and language model)
- **Pinecone** (vector database)
- **PyPDF** (PDF text extraction)
- **dotenv** (environment variable management)
  

---

# AI Meal Planner Agent
### [👉Click here to view the Live App](https://aimealplanneragent.streamlit.app/)

<p align="center">
  <img src="https://github.com/user-attachments/assets/23322977-2647-4e49-a86b-71271832a9a5" width="300" />
  <img src="https://github.com/user-attachments/assets/71fd7e60-feaa-4595-8975-7c2b6d824178" width="300" />
</p>

__________

## Summary

AI Meal Planner Agent is a Streamlit-based AI application that generates personalized meal plans from user-provided ingredients. The app uses OpenAI models to create healthy and structured meal recommendations based on calorie goals, meal preferences, and cooking styles.

Users can also:
- Download meal plans as PDF files
- Generate voice-guided cooking instructions
- Customize meals for breakfast, lunch, dinner, or full-day plans

---

## Why This Project Is Useful

This project helps users quickly create healthy meal plans without manually searching for recipes or calculating nutrition constraints.

It is useful for:
- People who want healthy meal suggestions
- Fitness-focused users tracking calories
- Users with limited ingredients at home
- Anyone interested in AI-powered productivity tools

The application combines AI-generated text, PDF generation, and AI voice synthesis into one interactive experience.

---

## Technologies Used

### Frontend / UI
- Streamlit

### AI Models
- OpenAI GPT-4.1-mini
- OpenAI Text-to-Speech (TTS)

### Backend / Logic
- Python

### PDF Generation
- ReportLab

### Other Python Libraries
- io.BytesIO

---

## Deployment

This project is deployed on Streamlit Cloud.

---

## Future Improvements

- Nutrition and macro tracking
- User authentication
- Saved meal history
- Multi-language support
- Grocery shopping list generation
- Database integration
- Image generation for meals

---
_____________________________________________________________________________________________________________________________________________________


# 4. 𝕏 Tweet Generator with Reflection Agents
An AI-powered tweet generation application built with LangGraph, LangChain, OpenAI, and Streamlit.
### [👉Click here to view the Live App](https://tweet-generator-langgraph.streamlit.app/)

<img width="1079" height="613" alt="Screenshot 2026-05-13 004104" src="https://github.com/user-attachments/assets/a4df0007-95de-47fb-9e10-de9878d2b224" />


This project uses a reflection-based workflow where the AI:
1. Generates an initial tweet
2. Critiques and reflects on the output
3. Improves the tweet iteratively
4. Produces a final optimized version

## Features

- AI tweet generation
- Reflection and self-improvement loop
- Multi-step draft iterations
- Final optimized tweet output
- Streamlit interactive UI
- LangGraph state-based workflow
- OpenAI GPT integration

## Tech Stack

- Python
- Streamlit 
- LangChain
- LangGraph
- OpenAI API

---

## Deployment

This project is deployed on Streamlit Cloud.

---

# 5. 🧠 Agentic Essay Writer

##  Project Overview

Agentic Essay Writer is an AI-powered essay generation application designed using an agentic workflow architecture. The system combines large language models, web research, iterative reflection, and revision mechanisms to generate high-quality essays dynamically.
### [👉Click here to view the Live App](https://agentic-essay-writer-k7.streamlit.app/)


<img width="1079" height="617" alt="1" src="https://github.com/user-attachments/assets/5022b38e-425d-4ac6-96be-59775f5d50d9" />


The application was built using:

- LangGraph
- LangChain
- OpenAI APIs
- Tavily Search API
- Streamlit

The goal of the project was to explore how multiple AI agents can collaborate within a structured workflow to perform planning, research, writing, critique, and revision tasks automatically.

---

#  Key Features

- AI-powered essay generation
- Multi-agent workflow orchestration
- Web research integration using Tavily
- Reflection and critique loop
- Iterative essay improvement
- Interactive Streamlit user interface
- Topic suggestion system
- PDF export functionality
- Configurable revision control
- GitHub-ready project structure

---

#  System Architecture

The project follows an agentic pipeline where multiple specialized agents interact through a state-driven workflow.

## Workflow

```text
User Input
   ↓
Planner Agent
   ↓
Research Agent
   ↓
Writer Agent
   ↓
Reflection/Critique Agent
   ↓
Revision Research Agent
   ↓
Improved Essay Generation
   ↓
Final Essay Output
```

---

# ⚙️ Technologies Used

| Technology | Purpose |
|---|---|
| LangGraph | Workflow orchestration |
| LangChain | LLM integration |
| OpenAI API | Essay generation |
| Tavily API | Web research |
| Streamlit | Frontend application |
| Python | Backend logic |
| FPDF | PDF export |
| Git & GitHub | Version control |

---

#  Core Components

## 1. Planning Agent

The planning agent generates a high-level essay outline based on the user's topic.

Responsibilities:
- Structure the essay
- Create logical flow
- Prepare writing guidance

---

## 2. Research Agent

The research agent generates search queries and retrieves relevant information from external web sources using Tavily Search.

Responsibilities:
- Gather contextual information
- Improve factual grounding
- Support essay generation with external knowledge

---

## 3. Writer Agent

The writer agent creates the essay using:
- User topic
- Essay outline
- Retrieved research content
- Critique feedback

Responsibilities:
- Generate coherent essays
- Integrate research context
- Improve writing quality iteratively

---

## 4. Reflection Agent

The reflection agent critiques the generated essay and provides recommendations for improvement.

Responsibilities:
- Analyze essay quality
- Identify weaknesses
- Suggest revisions
- Improve structure and depth

---

## 5. Revision Workflow

The application supports iterative refinement through a revision loop controlled by conditional graph routing.

Responsibilities:
- Re-research based on critique
- Regenerate improved drafts
- Control workflow iterations

---

# Potential Future Improvements

Future enhancements may include:

- Persistent database storage
- User authentication
- Essay history tracking
- Citation generation
- Vector database integration
- Semantic retrieval
- Multi-language support
- Async processing
- Advanced analytics dashboard
- Deployment scaling

---

#  Conclusion

Agentic Essay Writer represents a complete end-to-end AI engineering project that combines modern LLM workflows, agentic orchestration, retrieval integration, iterative reasoning, and frontend deployment into a unified intelligent application.

The project serves as both a practical AI product prototype and a strong demonstration of applied AI engineering concepts using modern open-source tooling and APIs.

_____________________________________________________________________________________________________________________________________________________
# 6. AI Finance Agent

> ⚠️ This is a personal and private project built for learning, research, and experimenting with AI-driven financial analysis and stock opportunity detection. The long-term goal is to create an intelligent finance agent for my own trading and investment research workflow. Since professional trading systems require strict financial logic, risk management, and validated strategies, this project is still evolving while I continue researching better trading theories, financial rules, and market analysis approaches.

This project is an AI-powered finance research and market scanning system that analyzes stocks, sectors, market trends, news sentiment, SEC filings, and company fundamentals to detect potential opportunities across the US stock market. It combines AI agents, vector databases, semantic SEC filing search, sector-based opportunity scoring, trend analysis, and Telegram alerts into one unified financial intelligence platform.

<img width="1067" height="611" alt="FA2" src="https://github.com/user-attachments/assets/9d0d4083-450b-4a57-9b8a-d7d5cd887110" />
<img width="1071" height="608" alt="FA3" src="https://github.com/user-attachments/assets/29a58d7a-73c9-49e2-a987-8aa7d507ae65" />
<img width="1079" height="515" alt="FA4" src="https://github.com/user-attachments/assets/87847920-bcf1-4f3c-9840-490a59311f1f" />
<img width="1072" height="408" alt="FA5" src="https://github.com/user-attachments/assets/e72bba68-3890-49f9-b8ee-71400285a53c" />
<img width="1079" height="611" alt="FA6" src="https://github.com/user-attachments/assets/216d84e9-8d93-49c6-a0b4-cd02e87a9ec2" />
<img width="1079" height="613" alt="FA7" src="https://github.com/user-attachments/assets/55caa395-51ac-41ab-aa06-ae39b782162f" />
<img width="1079" height="586" alt="FA8" src="https://github.com/user-attachments/assets/fe5e9633-7ea5-45ca-bee3-e348b4eaabc2" />


---

# Features

- AI-powered finance research agent
  - Ask natural language questions about stocks, risks, valuation, SEC filings, growth, and trends.

- SEC Filing RAG System
  - Downloads SEC filings (10-K)
  - Chunks and indexes filings into a vector database
  - Uses semantic search for official filing analysis

- Vector Search with ChromaDB
  - Stores embeddings of SEC filing chunks
  - Enables semantic retrieval instead of keyword-only search

- S&P 500 Market Scanner
  - Dynamically loads S&P 500 companies
  - Scans companies automatically
  - Detects potential market opportunities

- Sector Opportunity Scanner
  - Groups companies by sectors such as:
    - Technology
    - Healthcare
    - Financial Services
    - Energy
    - Real Estate
    - Utilities
    - Industrials
    - Consumer sectors
  - Ranks sectors by average opportunity score

- Opportunity Scoring Engine
  - Calculates custom opportunity scores using:
    - Revenue growth
    - Earnings growth
    - Trend analysis
    - News sentiment
    - Profitability
    - Valuation metrics
    - Debt analysis

- Trend & Momentum Analysis
  - Detects:
    - Strong upward trends
    - Weak trends
    - Momentum signals

- News Sentiment Analysis
  - Analyzes recent company news
  - Detects positive or negative market sentiment

- Telegram Alert System
  - Sends opportunity alerts directly to Telegram
  - Notifies strong or high-confidence opportunities

- Historical Scan Tracking
  - Stores previous scans
  - Detects score changes between scans

- Interactive Streamlit Dashboard
  - User-friendly finance dashboard
  - Sector exploration
  - Company inspection
  - AI research chat interface

---

# Technologies Used

## Core Technologies

- Python
  - Main backend language for the entire system

- Streamlit
  - Interactive frontend dashboard and UI

- OpenAI API
  - AI reasoning
  - Embeddings
  - Research generation
  - Semantic analysis

- ChromaDB
  - Vector database for SEC filing embeddings

- LangGraph
  - AI agent workflow orchestration

- LangChain
  - LLM tooling and agent integration

---

## Financial & Data Libraries

- yfinance
  - Stock market data
  - Company fundamentals
  - Financial metrics
  - Historical prices

- pandas
  - Data manipulation and analysis

- numpy
  - Numerical operations and calculations

- requests
  - API requests
  - SEC filing retrieval
  - Telegram communication

- beautifulsoup4
  - HTML parsing for SEC documents

---

## AI & NLP

- OpenAI Embeddings
  - Semantic vector embeddings for SEC filing search

- RAG (Retrieval-Augmented Generation)
  - Combines vector search with AI reasoning

- Semantic Search
  - Retrieves relevant filing context intelligently

---

## Notification & Automation

- Telegram Bot API
  - Real-time opportunity alerts

- dotenv
  - Secure environment variable management

---

# About SerpAPI Integration

A future improvement for this project is integrating SerpAPI to provide real-time stock market data and live financial information directly into the AI agent workflow.

At the time of development, my free SerpAPI credits were already exhausted. SerpAPI currently provides around 250 free API requests per month, which was not sufficient for large-scale market scanning and continuous agent-based analysis.


# Current System Workflow

---

```text
S&P 500 Companies
        ↓
Market Data Collection
        ↓
Trend + Fundamental Analysis
        ↓
News Sentiment Analysis
        ↓
Opportunity Scoring
        ↓
Sector Classification
        ↓
AI Research & SEC Filing Analysis
        ↓
Telegram Opportunity Alerts
```
_____________________________________________________________________________________________________________________________________________________

# 7. 🔎 AI Research Agent


AI Research Agent is a LangGraph-powered research assistant that generates structured research reports using ArXiv papers, web search, and RAG pipelines.  
It combines AI agents, vector search, and scientific paper ingestion to automate research workflows across multiple domains.

<img width="1079" height="554" alt="Research_Agent_3" src="https://github.com/user-attachments/assets/a5136da4-ab60-4072-9e13-9f8b7e3aa8c3" />
<img width="1079" height="617" alt="Research_Agent_1" src="https://github.com/user-attachments/assets/de61cda4-f27e-4fc4-a7dd-578863c35b91" />
<img width="1079" height="583" alt="Research_Agent_2" src="https://github.com/user-attachments/assets/c57f7459-0f33-4840-8b2b-50524dcf1f7c" />

---

## 🚀 Features

- AI-powered research report generation
- ArXiv paper ingestion & PDF processing
- RAG semantic search with Pinecone
- Web search integration using SerpAPI
- Multi-domain research support
- Interactive Streamlit interface

---

## 🛠️ Tech Stack

- Python
- LangGraph
- LangChain
- OpenAI API
- Pinecone
- Streamlit
- SerpAPI
- ArXiv API

---
## 🧠 Project Architecture

```text
                    ┌─────────────────────┐
                    │    User Question    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Streamlit UI        │
                    │                     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   answer_query()    │
                    │                     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ LangGraph Workflow  │
                    │   Oracle + Router   │
                    └──────────┬──────────┘
                               │
         ┌─────────────────────┼─────────────────────┐
         │                     │                     │
         ▼                     ▼                     ▼
 ┌──────────────┐     ┌──────────────┐     ┌──────────────┐
 │ rag_search   │     │ fetch_arxiv │     │  web_search  │
 └──────┬───────┘     └──────┬───────┘     └──────┬───────┘
        │                    │                    │
        ▼                    ▼                    ▼
 ┌──────────────┐    ┌──────────────┐    ┌──────────────┐
 │  Pinecone DB │    │    ArXiv     │    │   SerpAPI    │
 │ Vector Search│    │   Abstracts  │    │ Google Search│
 └──────┬───────┘    └──────────────┘    └──────────────┘
        │
        ▼
 ┌─────────────────────┐
 │    final_answer     │
 │ Structured Report   │
 └──────────┬──────────┘
            │
            ▼
      ┌────────────┐
      │   Output   │
      └────────────┘
```

---

## 📥 Ingestion Pipeline

```text
        ArXiv API
             │
             ▼
      Download PDFs
             │
             ▼
        Load PDFs
             │
             ▼
       Split Chunks
             │
             ▼
   OpenAI Embeddings
             │
             ▼
      Pinecone Vector DB
             │
             ▼
   Used by RAG Search Tools
```
