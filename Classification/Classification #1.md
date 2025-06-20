🧠 Student Classification: Time Management vs. Mental Health

This project analyzes student survey data to classify whether a student’s main concern is related to **time management** or **mental health**. The model is built using feature scoring and supervised learning techniques.

📂 Dataset
- Source: `student.csv` (survey responses)
- Features grouped into two categories:
  - **Time Management Related**
    - How much time spend in gaming?
    - When do you play the game most of the time during the day?
  - **Mental Health Related**
    - Do you feel hamper in sleep?
    - Do you feel the headache?
    - Do you feel mental stress?

### 🧮 Scoring System

| Original Response        | Score |
|--------------------------|-------|
| No                       | 0     |
| Sometimes                | 0.5   |
| Yes                      | 1     |
| <2 hours                 | 0     |
| 3-4 hours                | 0.5   |
| >5 hours                 | 1     |
| Morning                  | 0     |
| Evening                  | 0.5   |
| Mid-Night                | 1     |

- **Time_Management_Score** = Average of time-related scores × **1.5**
- **Mental_Health_Score** = Average of mental health-related scores × **1.0**

**Classification Rule**:
- If `Mental_Health_Score` > `Time_Management_Score` → `Mental Health`
- Else → `Time Management`

🤖 Models Used
- **Decision Tree Classifier** (max depth = 3)
- **Logistic Regression**

Both models were trained to classify students based on the weighted survey scores. The data was split into 70% training and 30% testing.

🌳 Decision Tree Insights

- Students reporting **more gaming hours**, **gaming late at night**, and **mild mental symptoms** were more often classified as **Time Management** cases.
- Students reporting **high levels of stress, fatigue, and headaches**, regardless of gaming, were labeled as **Mental Health**.
- **Midnight gaming** and **consistent "Yes" responses** on mental health indicators increase the likelihood of the mental health label.
