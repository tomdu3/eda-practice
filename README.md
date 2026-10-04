# EDA Practice

A collection of exploratory data analysis (EDA) notebooks and follow-along exercises, built with pandas, NumPy, matplotlib, seaborn and plotly. Datasets are pulled directly from Kaggle via `kagglehub`.

## Projects

### [eda-netflix](eda-netflix/)

EDA of a synthetic Netflix-style movie dataset (1,000,000 rows, 17 columns) covering genre, release year, budget, box office, IMDb/Rotten Tomatoes scores and votes.

- Notebook: [`eda-netflix.ipynb`](eda-netflix/eda-netflix.ipynb)
- Dataset: [Movie Dataset for Analytics and Visualization](https://www.kaggle.com/datasets/mjshubham21/movie-dataset-for-analytics-and-visualization) (downloaded to `eda-netflix/data/`)
- Resource: [YouTube walkthrough](https://www.youtube.com/watch?v=76PtvVqrRNo)

### [eda-sales](eda-sales/)

E-commerce sales and customer analytics, covering customer master data plus order, product and sales tables.

- Notebook: [`eda-sales.ipynb`](eda-sales/eda-sales.ipynb)
- Dataset: [E-commerce Sales and Customer Analytics](https://www.kaggle.com/datasets/datascikhan/e-commerce-sales-and-customer-analytics/data) (downloaded to `eda-sales/data/`)
- Resource: [Exploring Real-World Customer Data with Pandas](https://youtu.be/eGPcTHJ3ZxU)

### [eda-course](eda-course/)

Follow-along guides and activities from a structured EDA course, organised by course.

**course2 — Data structures, functions and missing data**

| Notebook | Topic |
| --- | --- |
| [`Activity_Discover what is in your dataset.ipynb`](eda-course/course2/Activity_Discover%20what%20is%20in%20your%20dataset.ipynb) | Activity: inspecting a dataset |
| [`Annotated follow-along guide_EDA structuring with Python.ipynb`](eda-course/course2/Annotated%20follow-along%20guide_EDA%20structuring%20with%20Python.ipynb) | Structuring data for EDA |
| [`Annotated follow-along guide_EDA using basic data functions with Python.ipynb`](eda-course/course2/Annotated%20follow-along%20guide_EDA%20using%20basic%20data%20functions%20with%20Python.ipynb) | Basic pandas data functions |
| [`Annotated follow-along guide_Date string manipulations with Python.ipynb`](eda-course/course2/Annotated%20follow-along%20guide_Date%20string%20manipulations%20with%20Python.ipynb) | Date/string manipulation |
| [`dealing_with_missing_data_lab/`](eda-course/course2/dealing_with_missing_data_lab/) | Dealing with missing data, outliers, input validation and label encoding |

**course3 — Sampling and probability distributions**

| Notebook | Topic |
| --- | --- |
| [`Annotated follow-along guide_ Sampling with Python.ipynb`](eda-course/course3/Annotated%20follow-along%20guide_%20Sampling%20with%20Python.ipynb) | Sampling techniques |
| [`Annotated follow-along guide_Work with probability distributions in Python.ipynb`](eda-course/course3/Annotated%20follow-along%20guide_Work%20with%20probability%20distributions%20in%20Python.ipynb) | Probability distributions |

## Setup

Python 3.12+ with dependencies managed by [uv](https://docs.astral.sh/uv/).

```sh
uv sync
```

Dataset downloads happen inside the notebooks via `kagglehub` and are written to each project's `data/` folder.

## Using virtual environment with ipython

- In order to use environment with uv, the ipython needs to be added:

```sh
uv add --dev ipython
```

- In order to use pyright and ruff inside neovim, activate the environment:

```sh
source .venv/bin/activate
```

## Instructional video

- [Have You Tried Running a Jupyter Notebook in Neovim](https://youtu.be/eIp31pLQ4sI)
