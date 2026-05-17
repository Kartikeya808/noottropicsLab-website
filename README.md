# README — `nootropiclab-frontend`

````md
# Nootropic Agent

An automated research ingestion pipeline that fetches neuroscience and cognitive-enhancement studies from PubMed and converts them into structured JSON for a live frontend.

This project powers the live research feed for Nootropic Lab.

---

## What It Does

- Fetches recent research papers from PubMed
- Extracts titles, abstracts, publication dates, and links
- Converts raw scientific data into structured JSON
- Powers a live deployed frontend
- Creates a foundation for AI summaries and semantic search

---

## Tech Stack

| Layer | Tech |
|---|---|
| Language | Python |
| Data Source | PubMed API |
| Parsing | XML + JSON |
| HTTP Requests | requests |
| Version Control | Git + GitHub |

---

## Architecture

```text
PubMed API
    ↓
Python Agent
    ↓
data.json
    ↓
Frontend Website
````

---

## Project Structure

```bash
.
├── advanced_pubmed_agent.py
├── pubmed_agent.py
├── scraper.py
├── data.json
├── requirements.txt
└── README.md
```

---

## Setup

### 1. Clone Repository

```bash
git clone https://github.com/Kartikeya808/nootropic-agent.git
cd nootropic-agent
```

### 2. Create Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install requests beautifulsoup4
```

### 4. Run The Agent

```bash
python3 advanced_pubmed_agent.py
```

The script generates:

```bash
data.json
```

which contains structured research data used by the frontend.

---

## Sample Output

```json
{
  "id": "42125501",
  "title": "Prenatal Methyl Nutrient Availability Shapes...",
  "abstract": "The dopaminergic system constitutes...",
  "pubdate": "2026",
  "link": "https://pubmed.ncbi.nlm.nih.gov/..."
}
```

---

## Why This Project Exists

Most scientific research is difficult to browse casually.

This project was built to create a cleaner and more accessible research discovery experience focused on:

* nootropics
* cognitive enhancement
* neuroscience
* emerging research

---

## Future Improvements

* Automated updates using GitHub Actions
* AI-generated summaries
* Relevance scoring
* Topic categorization
* Semantic/vector search
* RAG-based research assistant

---

## Frontend

Frontend repository:

[https://github.com/Kartikeya808/noottropicsLab-website](https://github.com/Kartikeya808/noottropicsLab-website)

Live website:

[https://nootropiclab.vercel.app/](https://nootropiclab.vercel.app/)

````

---

# README — `noottropicsLab-website`

```md
# Nootropic Lab

A lightweight research aggregation website focused on neuroscience, cognitive enhancement, and nootropics.

The site dynamically displays scientific studies fetched through a Python-based PubMed ingestion pipeline.

---

## Live Website

https://nootropiclab.vercel.app/

---

## Features

- Live research feed
- Dynamic study rendering
- Abstract previews
- Direct PubMed links
- Lightweight static frontend
- Automatically expandable architecture

---

## Tech Stack

| Layer | Tech |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Hosting | Vercel |
| Data Source | PubMed API |
| Backend/Data Pipeline | Python |
| Version Control | Git + GitHub |

---

## How It Works

```text
PubMed API
    ↓
Python Research Agent
    ↓
data.json
    ↓
Frontend fetch()
    ↓
Live Website
````

The frontend dynamically fetches research data from:

```text
https://raw.githubusercontent.com/Kartikeya808/nootropic-agent/main/data.json
```

---

## Local Development

### Clone Repository

```bash
git clone https://github.com/Kartikeya808/noottropicsLab-website.git
cd noottropicsLab-website
```

### Run Locally

Use VS Code Live Server or Python's local server:

```bash
python3 -m http.server
```

Then open:

```text
http://localhost:8000
```

---

## Future Improvements

* Search functionality
* Better UI/UX
* Category filtering
* AI-generated summaries
* Dark/light theme toggle
* Responsive research cards
* Infinite scrolling / pagination

---

## Backend Repository

Backend ingestion pipeline:

[https://github.com/Kartikeya808/nootropic-agent](https://github.com/Kartikeya808/nootropic-agent)

```
```
