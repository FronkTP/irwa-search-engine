# IRWA Final Project (2026) - Part 2: Indexing and Evaluation

## Project Overview

This repository contains Part 2 of the Information Retrieval and Web Analytics (IRWA) Final Project (2026). It focuses on building an inverted index, ranking documents using the TF-IDF algorithm, and evaluating the search engine's performance using standard information retrieval metrics.

**Git Tag:** `IRWA-2026-part-2`

## Requirements

Before running the notebook, ensure the data files are located in the main `data/` directory at the root of the project:

* `../../data/fashion_products_dataset.json`: The main dataset.
* `../../data/validation_labels.csv`: The provided ground truth validation labels for the two predefined queries.

## Directory Contents

* `part2.ipynb`: The main Jupyter Notebook containing the code for indexing, searching, ranking, and evaluation.
* `manual_test_relevance.csv`: A generated CSV file containing our manual, binary relevance judgments (Ground Truth) for our five custom test queries.
* `README.md`: This instruction file.

## How to Run the Code

Since this part of the project is entirely contained within a Jupyter Notebook, running the code is straightforward:

1. Launch Jupyter Notebook or Jupyter Lab from your terminal:
   ```bash
   jupyter notebook
   ```
2. Open the `part2.ipynb` file.
3. Select **Kernel > Restart & Run All** (or run the cells sequentially from top to bottom) to execute the data loading, text processing functions, and view the EDA plots and word clouds inline.
4. To test your own queries, locate the `test_queries` list in the notebook and modify or add new string queries. Rerun the subsequent cells to perform the conjunctive search and calculate the TF-IDF scores.

## AI Usage Acknowledgment

In accordance with the course's AI Usage Policy, we acknowledge the following use of AI tools in the development of this project submission:

* AI tools (such as ChatGPT) were used to assist in structuring this `README.md` file and formatting our documentation.
* AI was utilized as a brainstorming and debugging assistant during the development of the text indexing and evaluation pipeline (e.g., building evaluation functions logic).

All final code and explanations have been reviewed by the team.
