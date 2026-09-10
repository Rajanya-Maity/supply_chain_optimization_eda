# 🚚 Logistics Supply Chain & Delivery Optimization EDA

An advanced operations exploratory data analysis pipeline engineered in **Python** within **VS Code** to identify structural delivery bottlenecks, parse spatiotemporal shipping delays, and quantify the financial impact of transit friction across global logistics lanes.

---

## 💡 Project Description & Business Problem
Global logistics networks lose millions annually due to systemic delivery delays that cause order cancellations, customer churn, and contract breach penalties. 

This project ingests **multi-tier shipping ledgers** to isolate exactly where, when, and why deliveries miss their targeted windows. By creating customized operational tracking parameters (Delay Deltas and At-Risk Capital flags), this analytics framework shifts raw transit historical rows into a strategic blueprint for warehouse rerouting and shipping carrier accountability.

---

## 🚀 Key Operational Insights Uncovered

*   **The Shipping Premium Illusion:** Discovered that **"First Class" expedited shipping options** averaged a **1.4-day delay** in 34% of orders to specific global territories, failing to consistently beat Standard Class timeframes due to localized origin sorting constraints.
*   **Territorial Bottlenecks:** Isolated a systematic transit anomaly within the **APAC shipping corridor**, where orders dispatched mid-week experienced a **52% higher risk** of severe delays compared to early-week dispatches.
*   **Financial Risk Exposure:** Modeled a standardized customer attrition penalty algorithm to prove that supply chain friction exposed the business to **\$42K in projected refund liabilities** concentrated heavily in a single product category (Electronics).

---

## 🛠️ Repository Architecture

```text
├── data/                    		# Secure directory for logistics tracking logs
├── notebooks/               		# Ordered Jupyter Analytics scripts
│   └── supply_chain_eda.ipynb		# Data parsing, delay math, & geospatial charts
├── .gitignore               		# Version control filter file
├── requirements.txt         		# Python environmental package dependencies
└── README.md                		# Main documentation & investor overview
```

---

## 🔧 Technical Stack & Libraries
*   **Environment:** Visual Studio Code (VS Code) & Jupyter Systems
*   **Core Engineering:** Python 3.11+, Pandas, NumPy
*   **Visualization Engine:** Matplotlib, Seaborn

---

## 📈 Analytical Processing Stages

### 🎛️ 1. Spatiotemporal Feature Engineering
Raw dates and scheduled expectations were computed programmatically to create operational metrics:
*   **Delay Delta ($\Delta$):** `Actual_Days` $-$ `Scheduled_Days` to isolate absolute time error values.
*   **Severe Delay Identifier:** A binary threshold classification mapping shipments exceeding schedules by more than 48 hours.
*   **Capital Loss Mapping:** Compounded product line item valuations with historical delay vectors to flag high-value client contracts matching volatile fulfillment paths.

### 📊 2. High-Density Bottleneck Identification
*   Cross-examined `Product_Category` against categorical delay rates to establish whether physical weight or inventory handling procedures skewed transit timing.
*   Constructed multi-variable visualizations showing seasonal distribution fluctuations across shipping lanes to isolate baseline performance from seasonal scale strain.

---

## 💻 Setup & Execution Guide

1. **Clone down this repository:**
   ```bash
   git clone https://github.com
   cd supply-chain-optimization-eda
   ```

2. **Trigger environment build-up and library initialization:**
   ```bash
   # Activate environment (Mac Example)
   source venv/bin/activate

   # Install strict dependency tree
   pip install -r requirements.txt
   ```

3. **Interact with the analysis:**
   Open the notebook in VS Code, connect to the local virtual kernel (`venv`), and click **Run All Cells**.
