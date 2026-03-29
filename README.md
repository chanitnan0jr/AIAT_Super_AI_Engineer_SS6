# Super AI Engineer Season 6 - Hackathon Solutions

This repository contains solutions for **Super AI Engineer Season 6** hackathon challenges organized by the **Artificial Intelligence Association of Thailand (สมาคมปัญญาประดิษฐ์ประเทศไทย)** in March 2026.

---

## Project Overview

Three distinct hackathon challenges showcasing different AI/ML techniques:
- **Data Storytelling** — Exploratory analysis & visualization
- **Computer Vision (OCR)** — Election vote data extraction
- **Retrieval Augmented Generation (RAG)** — Intelligent document QA system

---

## Hackathon Challenges

### Hackathon 1: Data Storytelling with Fire Statistics
**File:** `Hackathon1/DataStoryTelling.ipynb`

#### Challenge Description
Analyze and visualize fire statistics data from Thailand (2019) to extract meaningful insights and propose mitigation strategies.

#### Key Techniques
- **Data Processing**: Pandas & NumPy for data manipulation and numerical computation
- **Data Cleansing & Preprocessing**: Handling Thai language encoding (UTF-8-sig), managing missing values, data normalization
- **Exploratory Data Analysis (EDA)**: Statistical summaries, distribution analysis, correlation studies
- **Visualization**:
  - Static visualizations using Matplotlib & Seaborn
  - Interactive visualizations using Plotly for enhanced exploration
- **Insights Generation**: Identifying fire patterns, risk zones, and seasonal trends
- **Strategy Proposals**: Recommending mitigation strategies based on findings

#### Key Sections
1. Setup & Load Data
2. Exploratory Data Analysis
3. Data Cleansing & Preprocessing
4. Advanced EDA & Insights
5. Proposed Mitigation Strategies

#### Tech Stack
- Python 3, Pandas, NumPy, Matplotlib, Seaborn, Plotly

---

### Hackathon 2: Typhoon OCR - Election Vote Extraction Pipeline
**File:** `Hackathon2/Typhoon_OCR.ipynb`

#### Challenge Description
Build an automated pipeline to extract election vote counts from scanned ballot images using OCR and AI reasoning.

#### Pipeline Architecture (4-Layer Design)

```
Layer 1: Setup
├── Install dependencies
├── Mount Google Drive
└── Configure API keys

Layer 2: OCR Processing
├── Typhoon OCR API
├── Image-to-text conversion
└── Save extracted text files

Layer 3: Reasoning & Extraction
├── DeepSeek V3.2 LLM
├── Parse vote counts (Id, Vote)
└── Generate CSV output

Layer 4: Submission
├── Merge with submission template
└── Format for competition
```

#### Key Techniques
- **Optical Character Recognition (OCR)**: Typhoon API for image text extraction
- **Large Language Models**: DeepSeek V3.2 for intelligent parsing and reasoning
- **Data Extraction**: Structured output generation (CSV format)
- **Pipeline Automation**: Automated workflow from image input to structured data

#### Tech Stack
- Python 3, Typhoon OCR API, DeepSeek LLM, Pandas

---

### Hackathon 3: FahMai RAG - Improved Retrieval Augmented Generation 
**File:** `Hackathon3/Fahmai_Rag_Improved.ipynb`

#### Challenge Description
Develop an intelligent FAQ/Policy lookup system using RAG (Retrieval Augmented Generation) with 8 key improvements over the baseline starter kit.

#### 8 Key Improvements

1. **Structured Chunking** — Intelligently split documents by Markdown headers instead of fixed-size chunks
2. **Metadata Enrichment** — Add brand and category metadata to every chunk for better context
3. **Question Extraction** — Clean and normalize user questions before retrieval
4. **Multi-Query Expansion** — LLM generates multiple question variations for comprehensive retrieval
5. **Query Router** — Intelligently route queries to specific policy/FAQ documents based on intent
6. **Product Focus Filter** — Prioritize relevant product documents when specific products are mentioned
7. **Cross-Encoder Reranking** — Re-rank retrieved chunks using semantic similarity
8. **Sibling Chunk Context** — Include related chunks for better answer quality

#### RAG Pipeline
```
User Query
    ↓
Question Extraction & Normalization
    ↓
Query Router (Intent Detection)
    ↓
Multi-Query Expansion (Generate variations)
    ↓
Dense Retrieval (Embedding-based search)
    ↓
Cross-Encoder Reranking
    ↓
Context Assembly (Sibling chunks)
    ↓
LLM Generation (Answer synthesis)
    ↓
Response
```

#### Tech Stack
- Python 3, sentence-transformers, pythainlp, rank-bm25, Pydantic
- LLM-based reasoning for intelligent retrieval and ranking

---

##  Repository Structure

```
AIAT_Super_AI_Engineer_SS6/
├── README.md                          # This file
├── Hackathon1/
│   ├── DataStoryTelling.ipynb        # Data analysis & visualization
│   ├── Readme.md                     # Hackathon 1 details
│   └── dataset/                      # Fire statistics dataset
├── Hackathon2/
│   ├── Typhoon_OCR.ipynb             # OCR pipeline implementation
│   └── Readme.md                     # Hackathon 2 details
└── Hackathon3/
    ├── Fahmai_Rag_Improved.ipynb     # RAG system implementation
    └── Readme.md                     # Hackathon 3 details
```

---

##  Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook or JupyterLab
- Dependencies listed in each hackathon notebook

### Installation

1. Clone the repository
   ```bash
   git clone <repository-url>
   cd AIAT_Super_AI_Engineer_SS6
   ```

2. Install dependencies (check each notebook for specific requirements)
   ```bash
   pip install pandas numpy matplotlib seaborn plotly
   pip install sentence-transformers pythainlp rank-bm25
   ```

3. Open notebooks in Jupyter
   ```bash
   jupyter notebook
   ```

---

##  Key Learnings

### Data Storytelling
- Effective data visualization for non-technical audiences
- Converting raw data into actionable insights
- Statistical analysis for decision-making

### Computer Vision & OCR
- Automating manual data entry with OCR technology
- Integrating multiple AI systems (OCR + LLM) in a pipeline
- Structured data extraction from unstructured sources

### Retrieval Augmented Generation
- Building intelligent QA systems without fine-tuning
- Improving search relevance through multiple techniques
- Combining embeddings, ranking, and LLM generation

---

##  Competition Context

All solutions were submitted for **Super AI Engineer Season 6** (Season 6, Year 2026), a comprehensive AI engineering competition focused on practical applications of machine learning and AI techniques.

**Event Date**: March 19-26, 2026
**Organizer**: Artificial Intelligence Association of Thailand

---

##  Notes

- Each hackathon notebook is self-contained and can be run independently
- Dataset links and additional resources are available in individual `Readme.md` files within each hackathon folder
- Solutions demonstrate best practices in Python programming, data science, and AI engineering

---

##  References

- [Artificial Intelligence Association of Thailand](https://www.thackle.or.th)
- Super AI Engineer Season 6 Official Website
- Individual hackathon notebooks for detailed implementation

---

**Last Updated**: March 30, 2026
**Status**: Competition Submissions Complete 
