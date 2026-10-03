# Vendor Invoice Intelligence System
**Freight Cost Prediction & Invoice Risk Flagging**

## 📌 Table of Contents

- <a href="#project-overview">Project Overview</a>
- <a href="#business-objectives">Business Objectives</a>
- <a href="#data-sources">Data Sources</a>
- <a href="#eda">Exploratory Data Analysis</a>
- <a href="#models-used">Models Used</a>
- <a href="#metrics">Evaluation Metrics</a>
- <a href="#application">Application</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#author--contact">Author & Contact</a>

---

<h2><a class="anchor" id="project-overview"></a>📌 Project Overview</h2>

This project implements an **end-to-end machine learning system** designed to support finance teams by:

1. **Predicting expected freight cost** for vendor invoices.
2. **Flagging high-risk invoices** that require manual review due to abnormal cost, freight, or operational patterns.

The system combines **Python, SQL, Pandas, Scikit-Learn, Joblib, and Streamlit** to create a complete machine learning workflow from data processing to deployment.

---

<h2><a class="anchor" id="business-objectives"></a>🎯 Business Objectives</h2>

### 1. Freight Cost Prediction (Regression)

Predict the expected freight cost of a vendor invoice based on invoice and purchase-related information.

**Business use cases:**

- Estimate expected freight expenses.
- Support budgeting and forecasting.
- Identify unusually high freight charges.
- Support vendor negotiations.
- Reduce manual freight-cost estimation.

### 2. Invoice Risk Flagging (Classification)

Identify invoices that may require manual approval based on abnormal invoice and purchasing patterns.

**Business use cases:**

- Detect potentially abnormal invoices.
- Reduce financial leakage.
- Prioritize invoices for manual review.
- Improve invoice approval workflows.
- Support finance and procurement teams.

---

<h2><a class="anchor" id="data-sources"></a>📂 Data Sources</h2>

The project uses an SQLite database containing vendor invoice and purchasing information.

### Main Tables

- `purchases`
- `purchase_prices`
- `vendor_invoice`
- `begin_inventory`
- `end_inventory`

The database is stored as:

```text
data/inventory.db