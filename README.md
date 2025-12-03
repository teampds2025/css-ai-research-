# Computational Social Science Analysis

This repository contains the code and analysis for a computational social science project investigating the formation of online communities around the intimate, creative, and relational uses of Large Language Models (LLMs).

The central goal is to understand how social norms and technical practices evolve within these niche subcultures on Reddit, particularly in response to major open-source model releases (e.g., Llama 2, Mixtral, Llama 3).

## Dataset
The analysis is based on a curated subset of the Pushshift Reddit Dataset, including both submissions and comments. It focuses on a curated set of subreddits and event-driven time periods relevant to the research question.  The initial event-driven dataset was strategically expanded to include inter-event baseline periods. This allows for a more robust comparative analysis that distinguishes between event-driven spikes and stable long-term community norms. The final corpus covers key months between December 2022 and April 2025.

## Repository Structure
The project follows the full research cycle. The current progress is documented in the `notebooks/` directory:
```
├── notebooks/
│   ├── 1_Download_and_Understand_a_Dataset/
│   │   ├── data_preparation.ipynb          # initial preparation, filtering, and basic cleaning 
│   │   └── metrics.ipynb                   # high-level metrics
│   │
│   └── 2_Exploratory_Data_Analysis_(part_1)/
│       ├── data_preparation_v2.ipynb       # revised data preparation notebook 
│       └── quality_checks.ipynb            # null/special value analysis and structural validation
│   │
│   └── 3_Exploratory_Data_Analysis_(part_2)/
│       └── eda.ipynb                       # the core EDA work
│   │
│   └── 4._Professional_Behavioural_Research_Report/
│       └── eda_text.ipynb                  # linguistic quality and modeling
│       └── pushshift_ai.model              # Word2Vec model
└── README.md
```

## Tech Stack
*   **Language:** Python 3
*   **Data Processing and Analysis**: Pandas, NumPy, scikit-learn, joblib, tqdm, re
*   **Visualization**: Matplotlib, Seaborn
*   **NLP and Modeling**: gensim, lingua, statsmodels
