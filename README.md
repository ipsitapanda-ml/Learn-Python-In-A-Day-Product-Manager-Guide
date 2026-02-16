# Learn Python In A Day Product Manager Guide
A Repo Designed For Product Managers To Learn Python in A Day

# Learn Python in a Day (Basics First → PM Use Cases)

This repo is a **one-day crash course**: you’ll cover Python fundamentals in the morning, then apply them to **product-style analytics** in the afternoon.

**Promise:** by the end, you can read a dataset, clean it, compute a few KPIs, and export something shareable.

---

## Setup (10 minutes)

### Option A — Google Colab (fastest)
- Open a notebook from `/notebooks`
- Run it in Colab (upload `data/events_sample.csv` when prompted)

### Option B — Local (recommended)
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook

