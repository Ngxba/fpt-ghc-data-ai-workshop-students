# AI Customer Support Intelligence — Student Workshop

Welcome to the **AI Customer Support Intelligence** hands-on workshop! In this workshop, you will connect relational databases, SQL analytics, interactive Plotly visualizations, OpenAI embeddings with `pgvector`, and build an intelligent customer support assistant.

## Learning Flow
| Section | File | Time | Activity |
|---|---|---:|---|
| 1 | `notebooks/01_data_etl_sql.ipynb` | 45m | Explore Kaggle support ticket sample -> Pandas cleaning -> PostgreSQL table + joins |
| 2 | `notebooks/02_dashboard_in_notebook.ipynb` | 25m | Define practical metrics & build interactive Plotly charts directly in notebook |
| 3 | `notebooks/03_embeddings_rag_openai.ipynb` | 50m | OpenAI embeddings -> team pgvector -> SQL retrieval -> grounded LLM answers |
| 4 | `notebooks/04_streamlit_app.ipynb` | 40m | Assemble complete Streamlit web UI prototype combining analytics & AI |
| 5 (Bonus) | `notebooks/05_bonus_langchain_agent.ipynb` | +30–45m | LangChain agent with tool routing for SQL metrics and RAG retrieval |

---

## Getting Started

### 1. Prerequisites
- Python 3.12 or 3.13
- [uv](https://docs.astral.sh/uv/) (recommended fast package manager) or standard Python `pip`

### 2. Setup environment with `uv`
Clone this repository and run:
```bash
# Automatically creates virtual environment and installs all dependencies
uv sync
```

### 3. Configure credentials
Copy the template file:
```bash
cp sample.env .env
```
Open `.env` and fill in the credentials provided by your instructor:
- `LAB_PROJECT_REF`: Supabase project reference
- `LAB_POOLER_HOST`: Transaction pooler host
- `LAB_TEAM_NUMBER`: Your assigned team number (e.g. `1`)
- `LAB_DB_PASSWORD`: Your team database password
- `OPENAI_API_KEY`: Provided OpenAI API key

### 4. Launch JupyterLab
```bash
uv run jupyter lab
```
Open `notebooks/01_data_etl_sql.ipynb` to begin Section 1!

---

## Helpful References
- Database Schema: [reference/schema_reference.sql](reference/schema_reference.sql)
- App Template: [app/streamlit_app.py](app/streamlit_app.py)
- Workshop Agenda: [Workshop_Syllabus_Detailed_Agenda.md](Workshop_Syllabus_Detailed_Agenda.md)
