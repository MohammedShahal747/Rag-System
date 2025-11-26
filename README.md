# 🚗 RagSystem1 – Agentic Car Analytics with RAG

RagSystem1 is a **Streamlit-based Agentic AI app** that analyzes car datasets and answers natural-language questions using:

- 🧼 **ETL Agent** – checks data quality  
- 📊 **Analysis Agent** – performs car-wise/brand-wise/segment-wise insights  
- 🧠 **RAG Agent** – Retrieval-Augmented Generation using ChromaDB  
- 📈 **Forecast Agent** – predicts future car sales (ARIMA / Linear Regression)  
- 🧭 **Recommendation Agent** – generates business suggestions

It’s optimized for **car data**: brands, models, segments, sales, terrain suitability, usage type (city / rural / highway), comfort rating, etc.

---

## ✨ Features

- 🧹 **Automatic ETL Check**
  - Counts rows, columns, missing values, and duplicates
  - Displays detected column names

- 📊 **Smart Car Analytics**
  - Finds best performing brands/segments/models
  - Computes average ratings and total sales
  - Compares brands, segments (SUV vs Sedan vs Hatchback, etc.)
  - Analyzes strengths of top car models

- 🧠 **RAG (Retrieval-Augmented Generation)**
  - Uses **ChromaDB** as a local vector store
  - You can paste car knowledge snippets (one per line) in the sidebar
  - System retrieves the most relevant snippets and enriches the answer

- 📈 **Forecasting**
  - Time-series forecasting for car sales using:
    - ARIMA(1,1,1) when available
    - Linear Regression as a fallback
  - Requires a time column like `Month`, `Date`, or `Year`

- 🧭 **Recommendations**
  - Generates high-level actions based on the analysis and forecast  
    (e.g., focus on top-performing segments, adjust strategy on decline, etc.)

- 🎨 **Modern UI**
  - Dark gradient theme
  - Colored result boxes for:
    - Normal answers
    - RAG-enhanced answers
    - Forecast outputs
    - Errors

---

## 🛠 Tech Stack

- **Python 3**
- **Streamlit** – UI & app framework
- **Pandas / NumPy** – data processing
- **ChromaDB** – vector database for RAG
- **scikit-learn** – Linear Regression
- **statsmodels** – ARIMA time-series model (optional)

---

