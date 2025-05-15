```markdown
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

```

📂 call-center-performance-analysis/
├── README.md                     # Project documentation
├── call\_center\_analysis.ipynb   # Jupyter notebook with full analysis
├── agent\_success\_rates.png      # Visual: Success rate per agent
├── total\_calls\_by\_agent.png     # Visual: Total calls by each agent
├── top\_agents.png               # Visual: Top 5 performing agents

````

---

## 📄 Dataset Overview

The dataset used for this analysis contains anonymized call performance metrics for individual agents. It includes the following columns:

- `Agent`: Name of the agent
- `Calls Made`: Total outbound calls made by the agent
- `Calls Answered`: Number of calls answered
- `Success Rate (%)`: Calculated as `(Calls Answered / Calls Made) * 100`

---

## 🧪 Analysis Workflow

### 1. Importing Data & Libraries

The project starts by importing essential libraries like `pandas`, `matplotlib.pyplot`, and `seaborn`, then loading the dataset into a DataFrame.

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
````

### 2. Calculating Success Rate

We create a new column, `Success Rate (%)`, that represents the percentage of successful call outcomes.

```python
df['Success Rate (%)'] = (df['Calls Answered'] / df['Calls Made']) * 100
```

### 3. Exploratory Data Analysis (EDA)

Several visualizations were created to extract insights, including:

* **Bar plot of total calls by agent**
* **Bar plot of agent success rates**
* **Top 5 agents with highest success rates**

Visuals are stored in the root directory:

* `total_calls_by_agent.png`
* `agent_success_rates.png`
* `top_agents.png`

### 4. Identifying Top Performers

We sorted the agents by success rate and isolated the top 5 performing agents:

```python
top_agents = df.sort_values(by='Success Rate (%)', ascending=False).head(5)
```

---

## 📈 Visualizations

Below are the visual highlights generated during the analysis:

* **Total Calls by Agent**: Shows how many calls each agent made
* **Agent Success Rates**: Displays conversion effectiveness
* **Top 5 Agents**: Highlights the most successful performers

All plots were styled with Seaborn for clarity and readability.

---

## 🔍 Insights & Key Takeaways

* Agents with high call volume don’t always have high success rates.
* Some agents are extremely efficient with fewer calls and higher conversion.
* There's an opportunity to coach underperforming agents based on the behavior of top performers.
* Visualizing performance helps uncover patterns not obvious in raw data.

---

## ▶️ How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/timelesshov/call-center-performance-analysis.git
cd call-center-performance-analysis
```

2. Launch the Jupyter Notebook:

```bash
jupyter notebook call_center_analysis.ipynb
```

3. Run all cells to view the analysis and charts.

---

## 🧠 What I Learned

Through this project, I improved my ability to:

* Handle real-world-style datasets with missing or varied data.
* Perform detailed performance analysis with Python.
* Visualize insights in a clear and actionable way.
* Communicate analytical findings effectively.

---

## ✍️ Author

**Stanley Chinor Okoro**
📍 Data Analyst | Python | SQL | Data Visualization
📧 [stanley.chinor@gmail.com](mailto:stanley.chinor@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/timelesshov)
🐙 [GitHub](https://github.com/timelesshov)

---

## 🪪 License

This project is licensed under the MIT License. You are free to use, modify, and distribute it.

---

## 🙌 Contributions

Contributions, suggestions, and feedback are welcome!

To contribute:

* Fork the repo
* Make your changes
* Open a pull request

---

```

Let me know if you'd like me to also generate:
- A `LICENSE` file (MIT)
- GitHub badges (e.g., `made-with-python`, `last-commit`)
- A `requirements.txt` file

Or help you prepare for other data analyst portfolio writeups.
```
