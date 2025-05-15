# 📞 Call Center Performance Analysis

This project provides a comprehensive analysis of call center agents' performance to help stakeholders identify strengths, weaknesses, and optimization opportunities within a customer support environment. The analysis is conducted using Python, leveraging powerful libraries like Pandas, Matplotlib, and Seaborn for data manipulation and visualization.

---

## 📌 Project Objective

The main objective of this project is to evaluate the performance of individual call center agents based on their call metrics — such as total calls made, calls answered, and success rates. This performance review provides actionable insights for improving operational efficiency, agent productivity, and customer service quality.

---

## 📊 Key Goals

- Clean and preprocess call center data.
- Calculate success rate of each agent.
- Visualize the performance of agents with informative charts.
- Identify top and bottom-performing agents.
- Highlight insights and recommend data-driven improvements.

---

## 🧰 Tools & Technologies Used

| Tool            | Description                                        |
|-----------------|----------------------------------------------------|
| **Python**      | Programming language used for analysis             |
| **Jupyter**     | Interactive environment for code and documentation |
| **Pandas**      | Data manipulation and analysis                     |
| **Matplotlib**  | Data visualization                                 |
| **Seaborn**     | Statistical data visualization                     |

---

## 📁 Project Structure
📁 call-center-performance-analysis
├── call_center_analysis.ipynb # Jupyter Notebook with full Python code
└── README.md # Project overview and documentation


---

## 📥 Dataset Description

The dataset includes the following key columns:

- `Agent`: The name of the call center agent  
- `Calls Made`: Number of outbound calls made  
- `Calls Answered`: Number of calls answered  
- `Success Rate (%)`: The success percentage calculated as `(Calls Answered / Calls Made) * 100`

---

## 🔍 Key Analysis & Visualizations

### ✅ 1. Success Rate Calculation

We calculated each agent’s success rate using:

```python
df['Success Rate (%)'] = (df['Calls Answered'] / df['Calls Made']) * 100

📌 Insights & Recommendations
Some agents demonstrate high efficiency with fewer calls but higher success rates.

Others make many calls but convert fewer — a coaching opportunity.

Success rate distribution shows clear outliers worth investigating.

Top agents could help mentor or train others.

