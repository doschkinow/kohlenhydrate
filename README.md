# Kohlenhydrate — Notebooks that estimate the amount of carbohydrates in a meal

This repository contains Jupyter notebooks for estimating carbohydrate-related data using different model/backends.

**Notebooks included**
- [anthropic-estimator.ipynb](anthropic-estimator.ipynb) — Example estimator using Anthropic-related tooling.
- [together-estimator.ipynb](together-estimator.ipynb) — Example estimator using Together.ai tooling.
- [usda-estimator.ipynb](usda-estimator.ipynb) — Estimator notebook based on USDA data sources.

**Purpose**
- Provide reproducible example notebooks for evaluating carbohydrate estimations in a meal.
- Offer lightweight reference implementations you can run and adapt.

**Prerequisites**
- Python 3.8+ (recommended)
- Jupyter or VS Code with the Jupyter extension
- (Optional) A virtual environment for isolation

**Quickstart**
1. Clone the repository and open it in VS Code or Jupyter Lab/Notebook.
2. (Optional) Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate   # macOS / Linux
.venv\Scripts\activate    # Windows (cmd / PowerShell)
```

3. Install dependencies if a `requirements.txt` file is present, otherwise install Jupyter:

```bash
pip install -r requirements.txt  # if present
pip install jupyterlab jupyter
```

4. Open the desired notebook (one of the three listed above) and run the cells.

**Notes**
- Since the notebooks reference external APIs (anthropic, together and usda) — configure configure them in a .env file like:
```
ANTHROPIC_API_KEY="..."
TOGETHER_API_KEY="..."
USDA_API_KEY="..."
```
- If you plan to reproduce results, pin package versions in a `requirements.txt` file.

**Contributing**
- Feel free to open issues or pull requests to add features, examples, or dependency files.

**License & Contact**
- Add a license file if you want to specify reuse terms.
- For questions, open an issue in this repository.
