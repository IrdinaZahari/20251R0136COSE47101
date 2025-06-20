🧠 Mental Health Classification (Dataset No. 2)

This classification is used to classify university students based on whether they are likely to **need mental health support**. The classification is based on academic, behavioral, and psychological factors derived from survey data.

 📂 Dataset
- Source: Preprocessed mental health survey dataset of university students
- Total records: ~27,000
- Features include:
  - GPA (categorized)
  - Academic Pressure
  - Study Satisfaction
  - Sleep Duration
  - Dietary Habits
  - Suicidal Thoughts
  - Work-Study Hours
  - Financial Stress
  - Family History

---

🧮 Scoring System

| Feature               | Mapping                                                                 |
|-----------------------|-------------------------------------------------------------------------|
| **GPA**               | Low: 0 (≤6.89), Average: 1 (6.90–8.56), High: 2 (≥8.57)                 |
| **Academic Pressure** | Low: 0 (score 1–2), Moderate: 1 (score 3), High: 2 (score 4–5)           |
| **Study Satisfaction**| Low: 0, Moderate: 1, High: 2                                             |
| **Sleep Duration**    | Very Short: 0, Short: 1, 7-8 Hours: 2, Long: 3                           |
| **Dietary Habits**    | Unhealthy: 0, Moderate: 1, Healthy: 2                                   |
| **Suicidal Thoughts** | Yes: 1, No: 0                                                            |
| **Work-Study Hours**  | Low (0–4h): 0, Average (5–8h): 1, High (9–12h): 2                         |
| **Financial Stress**  | Low (≤2): 0, Moderate (3–4): 1, High (5): 2                              |
| **Family History**    | Yes: 1, No: 0                                                            |

- **Total Score** = Sum of all individual scores  
- **Classification Rule**:
  - If `Total Score ≥ 6` → **"Yes"** (needs mental health support)
  - If `Total Score ≤ 5` → **"No"** (does not need support)

---

🤖 Models Used
- **Decision Tree Classifier** (`max_depth=3`, `class_weight='balanced'`)
- **Logistic Regression** (`class_weight='balanced'`)

Both models were trained on the computed scores and evaluated using a stratified 70/30 train-test split to preserve class balance.

---

🌳 Decision Tree Insights

The decision tree identified the following as key factors:
- **Work-Study Hours**: Students with **lower work-study hours** are not necessarily safe from mental health risk
- **Sleep Duration**: Students who sleep **very little or very long** are more likely to require support
- **Suicidal Thoughts**: A highly predictive feature — even in isolation, this leads to a "Yes" classification
- **Financial Stress** and **Family History** often increase risk when paired with other symptoms

🧠 Even students with:
- Low workload
- Long sleep duration
- No suicidal thoughts  
can still be flagged as needing support due to other correlating patterns in the data.
