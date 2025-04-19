# Educational AI & Equity: Supporting Fair Learning Analytics

This repository supports my ongoing research titled  
**"Embodied Reasoning and Algorithmic Mediation in Dynamic Mathematics Environments"**,  
prepared for submission to the 2025 PME-NA Conference.

## 📚 Project Overview

This project explores the intersection of **educational data mining**, **AI fairness**, and **mathematical cognition**. It investigates how intelligent tutoring systems (ITS) and adaptive platforms like Desmos and GeoGebra shape students' mathematical understanding especially their **embodied reasoning** and **affective engagement**.

---

## 🔍 Research Focus

- How do algorithms mediate reasoning and discovery in dynamic mathematics tools?
- What data features predict equitable or inequitable student engagement?
- How can design principles promote transparency and trust in AI-enhanced learning systems?

---

## 🧪 Sample Code: Detecting Patterns in Student Trajectories

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load sample interaction data
df = pd.read_csv('student_paths.csv')  # Example CSV: time, clicks, score, hint_usage

# Plot engagement over time
plt.figure(figsize=(10, 5))
plt.plot(df['time'], df['score'], label='Score')
plt.plot(df['time'], df['hint_usage'], label='Hint Usage')
plt.xlabel("Time (minutes)")
plt.ylabel("Score / Hints")
plt.title("Student Learning Trajectory")
plt.legend()
plt.grid(True)
plt.savefig('learning_trajectory.png')
plt.show()
```

---

## 📊 Example Visualization

![Sample Graph](learning_trajectory.png)  
_A line plot showing student score improvement and hint usage over time._

---

## 🔁 u-Substitution Pattern Detection Example

```python
import numpy as np

# Simulate u-substitution behavior
x = np.linspace(0.1, 5, 100)
u = x**2
f_x = 2 * x * np.cos(x**2)
f_u = np.cos(u)

# Compare original and transformed functions
plt.plot(x, f_x, label='f(x) = 2x·cos(x²)')
plt.plot(x, f_u, '--', label='f(u) = cos(u)')
plt.title('u-substitution Behavior (Symbolic)')
plt.xlabel('x')
plt.legend()
plt.grid(True)
plt.savefig('u_substitution_behavior.png')
plt.show()
```

---

## 🧠 Technologies Used

- Python: `pandas`, `numpy`, `matplotlib`
- Jupyter Notebooks for data analysis
- Educational platforms: Desmos API (simulated), GeoGebra exports
- Open-access educational datasets (or generated data for demo)

---

## 🚀 Future Directions

- Incorporate gesture-based reasoning logs from touchscreen interactions
- Explore fairness-aware student models and adaptive feedback loops
- Contribute to ethical AI policy in educational technology

---

## 📌 Citation

> Author: PhD Student in Applied Mathematics  
> Institution: Illinois Institute of Technology  
> Contact: easante@hawk.iit.edu
> Status: Research-in-progress for PME-NA 2025

---

Contributions and discussions welcome — especially from education researchers, developers, and policy advocates!

