# Learn Python in a Day (PM Edition)

A **quick, practical** Python guide for Product Managers: learn the **basics first**, then apply them to **product analytics** (KPIs, funnels, segmentation, exports).

This repo is beginner-friendly: short notebooks, lots of examples, and **synthetic (fake) datasets** included.

## What you’ll learn

### Part A — Python basics (first)
- Running Python in notebooks
- Data types: `int`, `float`, `str`, `bool`, `None`
- Variables + naming
- Operators: arithmetic + comparisons
- Type conversion: `int()`, `float()`, `str()`
- Strings: slicing + common methods (`lower`, `strip`, `split`, `replace`) + f-strings
- Collections:
  - Lists (add/remove/sort)
  - Tuples (immutability)
  - Sets (uniques)
  - Dictionaries (key/value, counting)
- Control flow:
  - `if / elif / else`
  - `for` loops (and light `while`)
  - practical patterns: filter, count, aggregate
  - comprehensions (list/dict/set)
- Functions:
  - `def`, parameters, defaults, return values
  - importing modules (`datetime`, etc.)
  - safe patterns (like avoiding divide-by-zero)

### Part B — Product-relevant topics (after basics)
- Data work with `pandas`:
  - load CSV (`read_csv`)
  - inspect (`head`, `info`, `describe`)
  - filter/select
  - clean missing values + types + timestamps
  - `groupby`, `agg`, `nunique`, `value_counts`
- PM analytics patterns:
  - DAU / WAU style metrics
  - funnel steps + conversion rates
  - revenue summaries (if revenue exists)
  - segmentation by plan / country / channel (if available)
  - lightweight cohort retention
- Reporting:
  - export to CSV
  - export to Excel (multi-sheet)

## Quick start

### 1) Clone the repo
git clone <your-repo-url>
cd <your-repo-folder>

### 2) Install dependencies
pip install -r requirements.txt

### 3) Start Jupyter
jupyter notebook

#### Notebook order (do these in order)

1. 01_basics_types_variables.ipynb

2. 02_strings_and_collections.ipynb

3. 03_conditionals_loops.ipynb

4. 04_functions.ipynb

5. 05_intro_to_pandas.ipynb

6. 06_pm_kpis_funnels.ipynb

7. 07_segmentation_retention.ipynb

8. 08_exports_csv_excel.ipynb

### Data (included)

This repo includes synthetic (fake) datasets so you can learn without using real company data.

#### 1. B2C app events

File: data/events_b2c_app.csv

Example funnel: app_install → app_open → signup → subscription_start (optional)

Common engagement events: session_start, content_view, share

#### 2. B2B SaaS events

File: data/events_b2b_saas.csv

Example funnel: account_created → trial_start → upgrade_to_paid

Common adoption events: project_created, integration_connected, invite_sent, login

Note: a small % of rows are intentionally messy (bad timestamps, missing values, inconsistent casing) so you can practice cleaning.

### Outputs (what “done” looks like)

When you finish the notebooks, you’ll generate files in the outputs/ folder, such as:

1- kpis_daily.csv

2- funnel_summary.csv

3- pm_report.xlsx

If those show up, you’re good ✅

### Troubleshooting (common beginner issues)

1- ModuleNotFoundError (e.g., pandas not found):

    pip install -r requirements.txt


2- jupyter: command not found:

    pip install jupyter

3- python or pip not found:

    Install Python from python.org, then reopen your terminal and try again.
