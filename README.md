# Computational Social Science: AI Subculture Analysis

This repository contains the code and analysis for a computational social science project investigating the formation of online communities around the intimate, creative, and relational uses of Large Language Models (LLMs).

The central goal is to understand how social norms and technical practices evolve within these niche subcultures on Reddit, particularly in response to major open-source model releases (e.g., Llama 2, Mixtral, Llama 3).

## Overview
The analysis is based on a curated subset of the Pushshift Reddit Dataset, including both submissions and comments. It focuses on a curated set of subreddits and event-driven time periods relevant to the research question.  The initial event-driven dataset was strategically expanded to include inter-event baseline periods. This allows for a more robust comparative analysis that distinguishes between event-driven spikes and stable long-term community norms. The final corpus covers key months between December 2022 and April 2025.

## Research Summary 
The methodology involved a multi-stage data processing pipeline, which included categorizing submissions and comments, identifying different types of content removal (self-censorship vs. moderation), and constructing a bot detection system combining text analysis with AI classification to filter out automated posts and focus on real human activity. To address the issue of linguistic quality, language identification, spam detection, and Word2Vec-based lexicon expansion were applied, with the final step being the use of topic modeling techniques (BERTopic).

## Technology Stack
Language: Python 3.11.9 (Required for compatibility with specific HDBScan/UMAP wheels). Key Libraries:

* **Data Processing**: Pandas, NumPy, PyArrow
* **NLP & Modeling**: BERTopic, Sentence-Transformers, Gensim (Word2Vec), Lingua-language-detector, PyTorch
* **Visualization**: Matplotlib, Seaborn, Plotly
* **Clustering**: HDBSCAN, UMAP-learn
*(See `requirements.txt` for full list)*

## Setup and Installation

1.  **Prerequisites:**
    *   Python 3.11.9
    *   Git

2.  **Clone Repository:**
    ```bash
    git clone https://github.com/teampds2025/css-ai-research-.git
    ```

3.  **Set Up Virtual Environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate
    ```

4.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

5. **Running the Analysis:**
    *   The repository contains Jupyter notebooks detailing the all operations performed, see `notebooks/`


## Repository Structure
The project follows the full research cycle. The current progress is documented in the `notebooks/` directory:
```
├── artifacts/    # BERTopic embeddings and Word2Vec model
│ 
├── figures/ 	  # BERTopic figures
│ 
├── notebooks/
│   ├── 1_Download_and_Understand_a_Dataset/ 	      # HW3
│   │
│   └── 2_Exploratory_Data_Analysis_(part_1)/	      # HW4
│   │
│   └── 3_Exploratory_Data_Analysis_(part_2)/	      # HW4
│   │
│   └── 4._Professional_Behavioural_Research_Report/  # HW5
│   │
│   └── 5._Final_Project_Presentation_&_Code/	      # EXAM
│ 
├── requirements.txt
│ 
└── README.md
```

## Dataset Link
Available at the [link](https://drive.google.com/drive/folders/1scQ0fZNXA6g10r8wZD1SBsujIhip3PDc?usp=sharing), contains all final datasets for each stage of analysis, respectively.
```

