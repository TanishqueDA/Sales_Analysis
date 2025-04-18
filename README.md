# 🛍️ Sales Data Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Colab](https://img.shields.io/badge/Colab-Google-yellow?logo=googlecolab)
![License](https://img.shields.io/badge/License-MIT-green)

An end-to-end data analysis project to explore trends, optimize marketing timing, identify top products, and predict sales using machine learning.

---

## 📁 Dataset

- **File**: `Sales_Data.csv`
- **Columns**: `Order ID`, `Order Date`, `Product`, `Quantity Ordered`, `Price Each`, `City`, `Purchase Address`, `Sales`
- **Source**: Synthetic or internal retail sales dataset

---

<details>
<summary><strong>📌 Key Steps</strong></summary>

### 📦 Data Preprocessing
- Removed nulls and fixed invalid entries (e.g., `"11-"` in date)
- Converted data types (`Order Date`, `Sales`, etc.)
- Feature engineering:
  - Extracted `Hour`, `Day of Week`, `State`
  - One-hot encoded `Product`, `City`, `State`
  - Created `Quantity * Price` interaction term
  - Scaled relevant numeric features

### 📊 Exploratory Data Analysis
- 📅 **Best Month for Sales**  
- 🏙️ **Top Cities by Sales**  
- ⏰ **Best Time for Ads** (10 AM–2 PM and 5 PM–9 PM)  
- 📦 **Top-Selling Products**
- 💸 **Price vs Quantity Correlation**

### 🧠 Machine Learning
- **Model**: Random Forest Regressor
- **Target**: `Sales`
- **Preprocessing**: Scaled numeric features + one-hot encoding
- **Evaluation**:
  - Mean Squared Error (MSE)
  - R² Score
- **Feature Importance**: Visualized most influential predictors of sales

</details>

---

## 📊 Visual Insights

| Chart | Insight |
|-------|---------|
| 📈 Monthly Sales | Seasonal spikes in sales |
| 🏙️ Sales by City | Top-performing regions |
| ⏰ Hourly Sales | Optimal times for advertising |
| 📦 Product Quantity vs Price | Demand is higher for cheaper products |
| 🌟 Feature Importance | Key factors impacting sales |

---

## ✅ Conclusion

- **Ads** should run mid-day and evening for max reach.
- **Lower-priced products** tend to drive more volume.
- **Sales prediction model** performs well using basic features + interactions.

---

## 🚀 Future Enhancements

- Interactive dashboards (Streamlit / Google Data Studio)
- Time-series sales forecasting
- Automated email reports and alerts

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| `Python`, `Pandas`, `NumPy` | Data handling |
| `Matplotlib`, `Seaborn` | Visualization |
| `Scikit-learn` | Machine learning |
| `Google Colab` | Execution environment |

---

## 📂 Project Structure

```bash
├── Sales_Data_Analysis.ipynb     # Jupyter Notebook
├── Sales_Data.csv                # Dataset
└── README.md                     # Project overview
