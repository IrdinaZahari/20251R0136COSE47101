tudent Time Management Classification (UniGame Dataset)

This classification is used to classify students based on whether they are likely to **need time management support**. 
The classification is based on survey features such as GPA, sleep patterns, class attendance, gaming habits, social time, and fatigue symptoms.

📂 Dataset
- Source: Preprocessed UniGame student behavior dataset
- Features:
  - Current CGPA (Low, Average, High)
  - Sleep timing (Healthy, Average, Late, Very Late)
  - Morning class attendance (Yes/No)
  - Average gaming time (Low, Moderate, High)
  - Time with family/friends (Low, Moderate, High)
  - Fatigue status (Yes/No)

🧮 Scoring System

| Feature                               | Mapping                        |
|---------------------------------------|--------------------------------|
| CGPA                                  | Low: 0, Average: 1, High: 2    |
| Sleep timing                          | Healthy: 0, Average: 1, Late: 2, Very Late: 3 |
| Morning class attendance              | Yes: 0, No: 1                  |
| Gaming time                           | Low: 0, Moderate: 1, High: 2   |
| Time with family/friends              | Low: 2, Moderate: 1, High: 0   |
| Fatigue                               | Yes: 1, No: 0                  |

- **Total Score** = Sum of all individual scores
- **Classification Rule**:  
  - Score **0–5** → `No` (Does not need time management help)  
  - Score **6 or more** → `Yes` (Needs time management help)

🤖 Models Used
- **Decision Tree Classifier** (max depth = 3)
- **Logistic Regression**

Each model was trained to predict the `Classification` label using the above features. Data was split into 70% training and 30% testing.

🌳 Decision Tree Insights

The decision tree revealed the following key patterns:
- Students with **low or average GPA** who **skip morning classes** and **spend less time socially** are more likely to need help.
- Students with **high GPA** but **moderate/high gaming time**, **fatigue**, and **poor sleep habits** are also often flagged as needing time management support.
- Even good academic performers can be at risk if their lifestyle habits are imbalanced.


