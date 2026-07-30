# 📊 StatInsight AI
### Enterprise Statistical Intelligence Platform for Bahrain

StatInsight AI is a production-ready AI-powered statistical intelligence platform built for processing, managing, and analyzing Bahrain's national statistical datasets.

The platform automatically ingests raw statistical files, transforms them into standardized master datasets, and enables users to explore data through natural language questions, interactive dashboards, and AI-generated insights.

Designed with scalability, security, and modularity in mind, StatInsight AI combines traditional data engineering with modern Large Language Models (LLMs) to provide fast, reliable, and intelligent statistical analysis.

---

# 🚀 Core Features

## AI-Powered Statistical Assistant

- Natural language question answering
- Hybrid regex + AI intent classification
- Context-aware statistical reasoning
- OpenAI fallback for complex analytical questions

---

## Intelligent Data Ingestion

Supports multiple ingestion methods:

- CSV uploads
- Apache Parquet files
- Base64 encoded datasets
- Remote URL imports
- Secure webhook ingestion

Incoming datasets are automatically:

- Validated
- Cleaned
- Normalized
- Mapped using configurable schemas
- Merged into master statistical datasets

---

## Statistical Query Engine

A high-performance analytical engine capable of:

- Filtering datasets
- Aggregations
- Grouping
- Trend analysis
- Time-series exploration
- Multi-dimensional statistical summaries

---

## Interactive Dashboard

Built using Gradio, the dashboard provides:

- Interactive charts
- Dynamic tables
- AI-generated summaries
- Natural language search
- Plotly visualizations

---

## Automated Data Pipeline

A background watcher continuously monitors incoming datasets and performs:

- Schema detection
- Column synonym mapping
- Duplicate detection
- Master dataset updates
- Automatic backups
- Validation checks

---

# 🏗 System Architecture

```
                    +----------------------+
                    |   Raw Data Sources   |
                    | CSV / Parquet / API  |
                    +----------+-----------+
                               |
                               |
                      Webhook / Upload
                               |
                               ▼
                +----------------------------+
                |   Data Ingestion Service   |
                +----------------------------+
                               |
                     Cleaning & Validation
                               |
                               ▼
               +------------------------------+
               | Master Statistical Datasets  |
               +------------------------------+
                               |
                               ▼
                 +--------------------------+
                 | Statistical Query Engine |
                 +--------------------------+
                               |
          +--------------------+--------------------+
          |                                         |
          ▼                                         ▼
   Regex Intent Router                    OpenAI LLM Engine
          |                                         |
          +--------------------+--------------------+
                               |
                               ▼
                    AI Response Generator
                               |
                               ▼
                    Interactive Gradio UI
```

---

# 🛠 Technology Stack

| Layer | Technology |
|--------|------------|
| Programming Language | Python 3.11 |
| User Interface | Gradio 6 |
| API Framework | Flask 3 |
| Data Processing | Pandas |
| File Format | Apache Parquet (PyArrow) |
| Visualization | Plotly |
| AI Models | OpenAI GPT Models |
| Search Integration | Bing Search API, SerpAPI |
| Containerization | Docker |
| Orchestration | Docker Compose |

---

# 📂 Project Structure

```
statinsight-ai/
│
├── app.py
├── Dockerfile
├── docker-compose.yml
│
├── config/
│   ├── endpoints.json
│   └── schemas.json
│
├── bahrain_agent/
│   ├── agent.py
│   ├── data_layer.py
│   ├── describe_layer.py
│   ├── nlu_router.py
│   └── query_layer.py
│
├── data/
│   ├── incoming/
│   ├── bahrain_master/
│   └── bahrain_master_backups/
│
└── scripts/
    ├── auto_ingest_watcher.py
    ├── webhook_receiver.py
    ├── ingest_and_prepare.py
    ├── fetch_and_ingest_replace.py
    └── check_masters.py
```

---

# ⚡ Getting Started

## 1. Clone the Repository

```bash
git clone <repository-url>
cd statinsight-ai
```

---

## 2. Configure Environment Variables

Copy the example configuration:

```bash
cp .env.example .env
```

Update the required variables:

```env
OPENAI_API_KEY=
WEBHOOK_SECRET=
SERPAPI_KEY=
BING_API_KEY=
```

---

## 3. Build the Containers

```bash
docker compose build
```

---

## 4. Start the Application

```bash
docker compose up -d
```

---

# 🌐 Services

| Service | URL |
|----------|-----|
| Gradio Dashboard | http://localhost:7860 |
| Webhook API | http://localhost:5000 |

---

# 📈 Data Processing Workflow

```
Upload Dataset
        │
        ▼
Validation
        │
        ▼
Column Mapping
        │
        ▼
Schema Normalization
        │
        ▼
Duplicate Detection
        │
        ▼
Master Dataset Merge
        │
        ▼
Backup Creation
        │
        ▼
Statistical Repository
        │
        ▼
AI Query Engine
```

---

# 🔒 Security Features

- Non-root Docker containers
- Webhook authentication
- Request validation
- MD5 duplicate detection
- File size restrictions
- Thread-safe ingestion
- Automatic master backups
- Secure environment configuration
- Input sanitization
- Rate limiting

---

# ⚙ Performance Optimizations

- In-memory repository layer
- Hybrid intent routing
- Cached dataset loading
- Optimized Parquet storage
- Lazy query execution
- Multi-stage Docker builds
- Efficient dataframe operations

---

# 📊 AI Capabilities

The platform combines deterministic statistical processing with Large Language Models to provide:

- Statistical summaries
- Trend analysis
- Dataset explanations
- Natural language querying
- Intelligent intent classification
- Context-aware analytical responses

---

# 🚀 Deployment

The platform is fully containerized and can be deployed using:

- Docker
- Docker Compose
- Linux VPS
- Cloud Virtual Machines
- Kubernetes (with minor configuration)

---

# 📄 License

This project is proprietary enterprise software developed for statistical intelligence and data analytics. Unauthorized redistribution or commercial use is prohibited without permission.

---

# 👨‍💻 Author

**StatInsight AI**

Enterprise Statistical Intelligence Platform

Built using Python, Flask, Gradio, Plotly, OpenAI, Pandas, and Docker to deliver scalable AI-powered statistical analytics.