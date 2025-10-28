
# 🧠 Differential Privacy on Census Data using PyDP

A Python project demonstrating how to apply **Differential Privacy (DP)** using the **PyDP (Python Differential Privacy)** library on the **UCI Adult Census Dataset**, with visualizations to analyze the impact of the privacy parameter (ε - epsilon) on data accuracy and noise.

---

## 📊 Overview

This project explores how differential privacy mechanisms affect statistical analysis.  
It computes **differentially private mean** and **count statistics** for key attributes like `age`, `hours-per-week`, and `education level`, comparing them to their true values for various epsilon values.

Through this project, you’ll:
- Understand how **epsilon (ε)** controls privacy vs. accuracy trade-offs.
- Visualize **Laplace noise** distribution and its impact on real data.
- Learn how to use **PyDP** to integrate DP in data pipelines.
- Generate insightful **plots and 3D visualizations** of noise and error propagation.

---

## ⚙️ Features

✅ Loads and cleans the **UCI Adult Census Dataset**  
✅ Computes true and DP-protected means and counts  
✅ Implements **Laplace mechanism** with bounded mean and count  
✅ Evaluates **error and relative error** between true and private statistics  
✅ Generates 2D and 3D visualizations

---

## 🧩 Libraries Used

| Library | Purpose |
|----------|----------|
| `pandas`, `numpy` | Data loading and processing |
| `seaborn`, `matplotlib` | Data visualization |
| `pydp` | Differential privacy computations |
| `mpl_toolkits.mplot3d` | 3D visualizations |

---

## 📂 Dataset

**UCI Adult Income Dataset**  
📍 Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data)

---

## 🚀 How to Run

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/differential-privacy-pydp.git
cd differential-privacy-pydp
```

### 2️⃣ Install Dependencies
```bash
pip install pandas numpy seaborn matplotlib pydp
```

### 3️⃣ Run the Script
```bash
python dp_analysis.py
```

---

## 🔒 Key Concept: Epsilon (ε)

- **Small ε (e.g., 0.1)** → Higher privacy, more noise, lower accuracy  
- **Large ε (e.g., 5.0)** → Lower privacy, less noise, higher accuracy  

This project quantifies and visualizes how changing ε affects mean and count estimations.

---

## 🧮 Example Results

| Epsilon | True Mean Age | DP Mean Age | Absolute Error |
|----------|----------------|--------------|----------------|
| 0.1 | 38.58 | 43.21 | 4.63 |
| 0.5 | 38.58 | 39.12 | 0.54 |
| 1.0 | 38.58 | 38.90 | 0.32 |
| 5.0 | 38.58 | 38.60 | 0.02 |

---

## 🧠 Learnings

- **Bounded mean** ensures DP-safe aggregation under known data limits.  
- **Laplace noise** adds randomness to preserve individual privacy.  
- The **privacy-utility tradeoff** can be visualized clearly through ε-variation.  

---

## 🏷️ Tags

`#DifferentialPrivacy` `#PyDP` `#DataPrivacy` `#MachineLearning`  
`#Python` `#DataAnalysis` `#Visualization` `#AI` `#UCI` `#PrivacyEngineering`

---

## 👨‍💻 Author

**Kripansh Kumrawat**  
📧 *[Your Email]*  
💼 [LinkedIn](https://linkedin.com/in/kripanshkumrawat) | [GitHub](https://github.com/your-username)
