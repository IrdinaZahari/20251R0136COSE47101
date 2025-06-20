📊 Project Summary

This classification aims to classify students into one of these two categories based on their responses to several questions : 
1. Mental Health issues
2. Time management issues

🕒 Survey Questions
Time Management Questions:
1. How much time spend in gaming?
2. When do you play the game most of the time during the day?

Mental Health Questions:
1. Do you feel hamper in sleep?
2. Do you feel the headache?
3. Do you feel mental stress?

🧮 Scoring System

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

- **Time Management Score** = Mean of related scores × 1.5  
- **Mental Health Score** = Mean of related scores × 1.0

Classification Label:
- `Mental Health` if `Mental_Health_Score` > `Time_Management_Score`
- `Time Management` otherwise
