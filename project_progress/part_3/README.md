# IRWA Final Project (2026) - Part 3: Ranking and Filtering

## Project Overview

This repository contains Part 3 of the Information Retrieval and Web Analytics (IRWA) Final Project (2026). It implements and compares multiple relevance ranking algorithms over a fashion e-commerce dataset.

**Git Tag:** `IRWA-2026-part-3`

## Requirements

Before running the notebook, ensure the data files are located in the main `data/` directory at the root of the project:

* `../../data/fashion_products_dataset.json`: The main dataset.

Required Python packages:
* Python 3.10+

```bash
pip install pandas numpy matplotlib nltk gensim jupyter
```

## Directory Contents

* `part3.ipynb`: The main Jupyter Notebook containing the code for indexing, searching, ranking, and evaluation.
* `manual_test_relevance.csv`: A generated CSV file for part 2 containing our manual, binary relevance judgments (Ground Truth) for our five custom test queries.
* `README.md`: This instruction file.

## How to Run the Code

Since this part of the project is entirely contained within a Jupyter Notebook, running the code is straightforward:

1. Launch Jupyter Notebook or Jupyter Lab from your terminal:
   ```shell
   jupyter notebook
   ```
2. Open the `part3.ipynb` file.
3. Select **Kernel > Restart & Run All** (or run the cells sequentially from top to bottom) to execute the data loading, text processing functions, building inverted index, precompute document norms, field lengths, vendor catalog statistics, and Word2Vec embeddings, then ranks matching products using each algorithm.
4. To adjust field importance, change the score in the  `FIELDS_WEIGHTS` variable in Part 2:

## Test Queries Evaluated

The notebook evaluates and compares all ranking methods on the 5 queries defined in Part 2:

1. `"women hoodie polycotton red graphic print"`
2. `"men wide blue v-neck t-shirt"`
3. `"summer dress pink"`
4. `"yellow running shoes"`
5. `"raincoat waterproof women"`

## AI Usage Acknowledgment

In accordance with the course's AI Usage Policy, we acknowledge the following use of AI tools in the development of this project submission:

* AI tools (such as ChatGPT) were used to assist in structuring this `README.md` file and formatting our documentation.
* AI was utilized as a debugging assistant during the development of the text ranking functions.

All final code and explanations have been reviewed by the team.
