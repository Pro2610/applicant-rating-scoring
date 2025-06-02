# Applicant Rating & Scoring System 🧮

This project presents a simple data-driven approach to evaluate and score loan or application submissions based on multiple criteria. The logic simulates a basic credit or priority scoring model.

## 🧩 Overview

The notebook performs the following key steps:

1. **Data Cleaning**  
   - Removal of duplicates based on applicant ID  
   - Filling missing values in external rating and education level  

2. **Rating Calculation**  
   Each applicant receives a score based on the following rules:
   - Age between 35 and 55 ➜ +20 points  
   - Applied on a weekday ➜ +20 points  
   - Married ➜ +20 points  
   - Location includes "Kyiv" or "Kyiv region" ➜ +10 points  
   - External rating ≥ 7 ➜ +20 points  
   - External rating ≤ 2 ➜ −20 points  
   - Applications with no amount or external rating = 0 ➜ score set to 0  

3. **Filtering Applications**  
   Only applicants with a score > 0 are selected for further consideration.

4. **Weekly Trends**  
   Submission dates are grouped by week to analyze average external ratings over time.

## 📊 Example Output

The notebook prints:
- First few rows of cleaned data  
- Ratings per applicant  
- Weekly average ratings  
- (Optional) A chart visualizing rating trends by week  

## 🔧 Tools & Libraries

- Python 3.x  
- pandas  
- matplotlib (optional, for visualization)

## 📁 Data

This project uses fictional sample data for demonstration purposes. You can adapt it to real-world datasets such as job applications, loan applications, or client assessments.

## 📌 Use Cases

This approach can be applied to:
- Lead qualification  
- Credit scoring models  
- Applicant prioritization  
- Internal ranking systems

## ✅ Author

Developed by [Yana Prozhuhan] as a personal data analytics project.  
Feel free to fork, adapt or contribute!# applicant-rating-scoring
