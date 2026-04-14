# 🛠️ Local Environment Setup (uv + Python 3.12.9)

## 📌 Overview

This project uses:

* `uv` for dependency and environment management
* A virtual environment (`.venv`) pinned to **Python 3.12.9**
* `pyproject.toml` for dependency tracking

---

## 🚀 When you open this repository

### ✅ In VS Code (recommended)

The environment is **auto-activated**.

You should see:

```bash
(learn_dbt)
```

👉 If you see this, you’re ready to work — no setup needed.

---

## 🔍 Verify environment (quick check)

```bash
python --version
```

Expected:

```bash
Python 3.12.9
```

---

## ⚠️ If environment is NOT activated

Run manually:

```bash
source .venv/Scripts/activate
```

---

## 📦 Install / sync dependencies

```bash
uv sync
```

👉 This installs all dependencies from `pyproject.toml`

---

## ▶️ Running commands (recommended)

Use `uv run` for clean execution:

```bash
uv run dbt build
```

or

```bash
uv run dbt run
```

---

## 🧩 Workflow Summary

```bash
# Open repo → open terminal (auto-activated)

uv sync          # only if dependencies changed
uv run dbt run   # run dbt
```

