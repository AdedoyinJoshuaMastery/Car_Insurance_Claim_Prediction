# Car Insurance Claim Prediction

## Overview
Insurance companies invest significant resources into optimizing pricing and estimating the likelihood of claims. In many countries, car insurance is legally required, making the market both large and competitive.  
On the Road Car Insurance requested a predictive model to estimate whether a customer will make a claim during their policy period. Since they have limited infrastructure for deploying complex machine learning systems, the initial goal is to identify the single most predictive feature that yields the highest accuracy. This project demonstrates skills in data preprocessing, exploratory analysis, and model evaluation.

## Project Instructions
The task is to identify the single feature of the dataset that best predicts whether a customer will make a claim (`outcome` column), excluding the `id` column.  
The final output is stored as a DataFrame called **`best_feature_df`**, containing two columns:
- `best_feature` → the name of the most predictive feature  
- `best_accuracy` → the accuracy score achieved using that feature  

This ensures a simple, interpretable model that can be deployed quickly.

## Dataset
The dataset `car_insurance.csv` contains customer demographic, financial, and driving history information. The target variable is `outcome`, which indicates whether a customer made a claim.

### Columns and Descriptions
| Column              | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `id`                | Unique client identifier                                                   |
| `age`               | Client's age group: 0 = 16–25, 1 = 26–39, 2 = 40–64, 3 = 65+               |
| `gender`            | Client's gender: 0 = Female, 1 = Male                                      |
| `driving_experience`| Years of driving: 0 = 0–9, 1 = 10–19, 2 = 20–29, 3 = 30+                   |
| `education`         | Education level: 0 = No education, 1 = High school, 2 = University         |
| `income`            | Income level: 0 = Poverty, 1 = Working class, 2 = Middle class, 3 = Upper class |
| `credit_score`      | Credit score (between 0 and 1)                                             |
| `vehicle_ownership` | Vehicle ownership: 0 = Financing, 1 = Owns vehicle                         |
| `vehicle_year`      | Vehicle registration year: 0 = Before 2015, 1 = 2015 or later              |
| `married`           | Marital status: 0 = Not married, 1 = Married                               |
| `children`          | Number of children                                                         |
| `postal_code`       | Client's postal code                                                       |
| `annual_mileage`    | Miles driven annually                                                      |
| `vehicle_type`      | Type of car: 0 = Sedan, 1 = Sports car                                     |
| `speeding_violations`| Number of speeding violations                                             |
| `duis`              | Number of DUI incidents                                                    |
| `past_accidents`    | Number of past accidents                                                   |
| `outcome`           | Claim status: 0 = No claim, 1 = Made a claim                               |

## Skills Demonstrated
- Data cleaning and preprocessing
- Exploratory data analysis
- Feature importance evaluation
- Model selection and accuracy comparison

## Files
- `notebooks/project.ipynb` → Jupyter Notebook with code
- `instructions/project_instructions.pdf` → Original project brief
- `requirements.txt` → Dependencies

## Results
The analysis identifies the single most predictive feature for claim likelihood, providing a simple yet effective starting point for deployment. This approach balances accuracy with ease of implementation for real-world use.

## License 
This project is licensed under the MIT License.

