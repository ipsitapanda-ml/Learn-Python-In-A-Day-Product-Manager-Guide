# Synthetic datasets (beginner-friendly)

This repo includes **synthetic (fake) datasets** so you can learn Python and product analytics without using real company data.

Put these files in the `data/` folder:

---

## 1) B2C app events
**File:** `events_b2c_app.csv`

**What it simulates:** a consumer app with installs, engagement, signup, and optional subscription.

**Typical funnel:**
`app_install → app_open → signup → subscription_start (optional)`

**Common engagement events:**
`session_start`, `content_view`, `search`, `share`, `add_to_cart`, `purchase`

**Useful beginner exercises:**
- DAU/WAU
- top events
- funnel conversion
- revenue by plan / country / channel
- basic cohort retention (by first week seen)

---

## 2) B2B SaaS events
**File:** `events_b2b_saas.csv`

**What it simulates:** account-based SaaS with trials, upgrades, usage, and occasional seat expansion.

**Typical funnel:**
`account_created → trial_start → upgrade_to_paid`

**Common adoption events:**
`project_created`, `integration_connected`, `invite_sent`, `login`, `report_viewed`, `export_csv`

**Useful beginner exercises:**
- trial → paid conversion (by channel / country)
- account activity (weekly active accounts)
- seat expansion / revenue moments
- adoption metrics (invites, integrations, report views)

---

## Columns (high-level)

### B2C file includes:
- `user_id`, `ts`, `event_name`
- `plan`, `country`, `channel`, `device`, `revenue`

### B2B file includes:
- `account_id`, `user_id`, `ts`, `event_name`
- `plan`, `country`, `channel`, `device`, `seats`, `revenue`

---

## Intentional “messiness” (for cleaning practice)
A small % of rows are intentionally imperfect:
- invalid / missing timestamps
- inconsistent casing / extra whitespace in `event_name`
- missing values in fields like `plan` or `country`
- `revenue` sometimes blank or stored as a string

That’s on purpose — beginners should learn how to clean data before analyzing it.
