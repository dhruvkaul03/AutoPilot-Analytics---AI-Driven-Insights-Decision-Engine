🚀 AutoPilot Analytics
AI-Driven Insights & Decision Engine for Small Businesses

A hybrid Computer Science + AI systems project focused on algorithms, data engineering, and real-world business impact.

⭐ Overview

Small and mid-sized businesses collect a tremendous amount of data—orders, customers, marketing performance, web traffic—but lack the engineering or data science infrastructure to turn that information into actionable decisions.

AutoPilot Analytics solves this problem.

This system is an end-to-end AI-powered analytics engine that:

Ingests and normalizes raw business data

Builds a metrics/semantic layer on top of a data warehouse

Detects anomalies, trends, and performance changes using algorithms

Uses multi-agent LLM reasoning to generate natural-language insights

Enables natural language → SQL querying

Provides a full dashboard for KPIs, insights, and explanations

This project blends core CS concepts (algorithms, databases, systems architecture, concurrency) with AI/ML engineering and practical business value.

⭐ Key Features
🔹 1. Data Ingestion Layer

Modular adapters for mock Shopify/Stripe/Analytics data

ETL pipeline (extract → transform → load)

Async ingestion + scheduling

Input validation + logging

🔹 2. Data Warehouse + Semantic Metrics Layer

Star schema (fact tables + dimension tables)

Clean definitions of key KPIs:

Revenue, AOV, ROAS, CAC, LTV, retention, churn

Automatic metric computation + caching

🔹 3. AI Insight Engine (Multi-Agent Reasoning)

Four cooperating agents:

Metric Scanner Agent — detects trends, anomalies, breakpoints

Insight Agent — converts math into natural-language explanations

Root Cause Agent — identifies drivers behind metric changes

Action Agent — suggests budget shifts and tactical recommendations

🔹 4. Natural Language → SQL Query Engine

Schema-aware question parsing

SQL generation with constraints

Query plan validation

Returns both chart-ready data & an explanation

🔹 5. REST API (FastAPI)

Endpoints for ingestion, metrics, insights, analysis, and querying.

🔹 6. Frontend Dashboard (React / Next.js)

KPI cards

Trend charts

Insight feed

NL-to-SQL chat interface

Segment analysis visualizations

⭐ Architecture Overview

AutoPilot Analytics is divided into 6 main layers:

┌──────────────────────────────┐
│       Frontend (Next.js)     │
└───────────────▲──────────────┘
                │
┌───────────────┴──────────────┐
│        FastAPI Backend        │
│  (Routing, auth, business API)│
└───────────────▲──────────────┘
                │
┌───────────────┴──────────────┐
│   AI Insight Engine (Agents)  │
│  - Scanner / Insight / RCA    │
│  - Planner / Recommender      │
└───────────────▲──────────────┘
                │
┌───────────────┴──────────────┐
│  Natural Language Query Engine│
│   (Parser → SQL → Validator)  │
└───────────────▲──────────────┘
                │
┌───────────────┴──────────────┐
│ Data Warehouse + Metrics Layer│
│  (Star Schema + Transformations)
└───────────────▲──────────────┘
                │
┌───────────────┴──────────────┐
│      Ingestion Pipelines      │
│   (ETL + mock API loaders)    │
└───────────────────────────────┘


This architecture demonstrates systems design, algorithms, data modeling, NLP, AI reasoning, and software engineering.

⭐ Why This Project Is Important (Business Perspective)

Businesses often have:

scattered data

disconnected dashboards

no systematic way to detect issues

no clear understanding of what’s driving performance

no data team to interpret trends

AutoPilot Analytics:

centralizes all data into one model

automatically analyzes metrics

flags anomalies instantly

explains what caused changes

recommends actions

This meaningfully reduces time spent manually investigating data issues and helps small teams make faster, better decisions.

⭐ Technologies Used
Backend

Python

FastAPI

PostgreSQL / DuckDB

Asyncio / Celery

Pandas / Polars

AI

OpenAI / Llama / Mistral APIs

Custom prompting

Multi-agent patterns

Frontend

React / Next.js

TailwindCSS

Chart.js or Recharts

Infrastructure

Docker (optional)

GitHub Actions CI (optional)

⭐ Getting Started
1. Clone the repo
git clone https://github.com/yourusername/AutoPilot-Analytics.git
cd AutoPilot-Analytics

2. Install dependencies
pip install -r requirements.txt

3. Initialize the database
python scripts/setup_db.py

4. Start the backend
uvicorn backend.api.main:app --reload

5. Start the frontend
npm install
npm run dev

⭐ Future Enhancements

Budget optimization using bandits (UCB / Thompson Sampling)

Customer lifetime value forecasting

Multi-tenant architecture

Live Shopify/Stripe integration

Agent memory for long-term tracking

⭐ Demo

(Coming soon — after you build the dashboard and API.)

⭐ Author

Dhruv Kaul
UIUC Statistics + Data Science
