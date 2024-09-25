# Health Tips Recommendation System

## Overview
This project implements a content-based recommendation system that suggests personalized health tips based on user profiles, such as age, gender, and medical history. The system uses Cosine Similarity to identify similar users and recommend the top three health tips relevant to each user.



## Dataset
The dataset used in this project includes user profiles with attributes such as age, gender, medical history, and recommended health tips. The dataset contains over 1000 rows, providing a diverse range of health conditions and demographics.

## Key Preprocessing Steps:
### Categorical Data Encoding:
- OneHotEncoder: Transforms variables like "Gender," "Medical Condition," and "Test Results" into numerical values.
- LabelEncoder: Applied to variables like "Doctor" and "Hospital" to facilitate comparisons between users.
### Numerical Data Scaling:
- StandardScaler: Normalizes features like "Age" and "Billing Amount" to ensure comparability and prevent bias in similarity calculations.
## Model Choice
The content-based recommendation system uses Cosine Similarity to measure the angle between user profile vectors, effectively capturing the similarity between profiles. This approach is particularly well-suited for high-dimensional data, such as user demographics and medical history.

### Why Cosine Similarity?
Cosine Similarity is ideal for this task because it focuses on the orientation (angle) between vectors rather than their magnitude, making it a robust choice for identifying users with similar health profiles.

## Model Implementation
- Similarity Matrix: Calculated between user profiles to identify the top three most similar users.
- Recommendation Generation: Extracted health tips associated with these similar users and recommended them to the target user, ensuring diversity by filtering out duplicates.
## Model Evaluation
The system's effectiveness was evaluated by comparing the recommended tips to the users' original health advice. While the model successfully recommended relevant health tips like Ibuprofen and Penicillin, it encountered challenges with duplicate recommendations.

## Suggested Improvements:
- Avoid Duplicate Recommendations: Implement a more advanced filtering system.
- Incorporate Collaborative Filtering: Analyze patterns from multiple users with similar health conditions to enhance recommendations.
- Use More Demographic Data: Include additional user information (e.g., lifestyle, diet) to refine recommendations.
## Performance Metrics
- Cosine Similarity Score: Used to identify the most similar users based on profile attributes.
- Real-Life Health Evaluation: Recommendations generally aligned with original health tips but require further validation against medical guidelines.
## Conclusion
The project demonstrates the effectiveness of a content-based recommendation system using Cosine Similarity for health tip recommendations. Future work will focus on expanding the dataset, incorporating collaborative filtering, and refining the evaluation process to ensure the practical, real-world applicability of the health tips provided.





# Tools/Software:
### Data Handling and Visualization:
➢ Libraries: NumPy, pandas, Matplotlib, Seaborn.

### Preprocessing and Modeling:
➢ Libraries: Scikit-learn, Statsmodels.

# Files to be uploaded in the repository:
1. Dataset --> healthcare.csv and Building a Simple Recommendation System for Health Tips.pdf
2. Code --> Healthcare.ipynb and Report on Health Tips.docx


