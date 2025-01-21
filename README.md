# Risk-Based Access Control Overview

- Mohamed Anwar Es-Safar
- Ibtissam Lahlou

Risk-Based Access Control (RBAC) is a security approach that evaluates the risk level associated with a user's access request in real-time. Instead of assigning static permissions, this method adapts to dynamic scenarios by considering various factors such as user behavior, location, device type, and historical data. The goal is to prevent unauthorized access, mitigate identity threats, and enhance system security without compromising usability. This approach is already implemented by [IAM venderos](https://learn.microsoft.com/en-us/entra/id-protection/concept-identity-protection-policies).

## What Was Achieved in This Project
This project focused on implementing machine learning techniques to detect identity-based threats, particularly account takeovers. The work involved analyzing a dataset of login attempts, which contained detailed information such as user device types, operating systems, browser details, geographical locations, and timestamps.

## Key steps included:

- Data Preprocessing and Exploration: The dataset was thoroughly examined to identify patterns and anomalies in login behavior, such as unusual login locations or devices.
- Risk Factor Identification: Various features were identified as indicators of risk, including IP connection frequency, ASN counts, and login success rates. These factors were used to characterize normal and suspicious activity.
- Addressing Imbalanced Data: Given the rarity of account takeovers compared to normal logins, strategies like oversampling were employed to balance the dataset and ensure effective model training.
- Feature Engineering: Categorical data such as countries, browsers, operating systems, and devices were encoded into numerical formats, while numerical data was scaled to enhance model performance.
Model Training and Validation: A machine learning model was trained using these engineered features to predict whether a login attempt was an account takeover. The model's performance was evaluated using metrics such as accuracy, precision, recall, and F1-score.


Overall, the project demonstrated the use of data-driven methods to enhance security by dynamically assessing the risk associated with user access requests, helping to prevent unauthorized activity while maintaining accessibility for legitimate users.