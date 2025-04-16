# Assignment_11
The coding and the readme files for "What drives the price of a car"
What drives the price of a car?
Background - The original dataset contained information on 3 million used cars. The provided dataset contains information on 426K cars to ensure speed of processing. There is no clear understanding of factors that determine the car prices.  
Goal- To understand what factors make a car more or less expensive and provide clear recommendations to clients (used car dealership) as to what consumers value in a used car.
Approach – The dataset initially contained several inconsistencies and irrelevant entries, including blank spaces, "NAN" values, and ambiguous terms like "Unknown" and "Other," which required extensive cleaning. Additionally, it included data on cars manufactured as early as 1900, which was not relevant since car dealers typically do not handle vehicles that old. To refine the dataset, I filtered it to include only cars produced between 2000 and 2020. These preprocessing steps ensured the dataset was more suitable for modeling and analysis, focusing on relevant and meaningful information.
Model – The dataset was modeled with two different regression models: multiple linear regression model (MODEL 1) with both numerical and categorical predictors (MODEL 2), as well as linear regression using X_train and X_test data structure. 
Findings - Formula vs. Feature Selection:
o	Model 1 uses a formula (formula) to specify the model, including both numerical and categorical predictors. It leverages statsmodels' ability to handle categorical variables with the C() function.
o	Model 2 explicitly selects features using column names (X = df_cleaned[['year', 'odometer', 'cylinders']]). It only uses numerical features and does not include categorical predictors in this specific implementation.
2.	Statistical Output:
o	Model 1, using statsmodels, provides a comprehensive statistical summary with p-values, R-squared, and other statistical measures.
o	Model 2, using sklearn, focuses more on prediction and provides metrics like mean squared error (MSE) and R-squared but might not give as much statistical detail.

Summary:
The suitability of a model largely depends on the specific goals you aim to achieve. A model's effectiveness is determined by how well it aligns with the objectives and requirements of the task at hand.
•	For statistical inference and understanding the relationships between variables: Model 1 (statsmodels) is generally preferred.
•	For prediction and model evaluation with potentially more complex feature engineering: Model 2 (sklearn) is often more suitable.
In this case the linear regression model is a better choice.

 
Recommendation to Car Dealers
1.	Highest sales categorically belong:
a.	Latest model (newer)
b.	full-size cars
c.	lower millage (odometer) 
d.	clean title_status
e.	Cars that are marked as “Excellent” or “Like New” sell quicker

2.	Additional factors include:
a.	More powerful cars with higher number of cylinders such as “6” or “8” have a higher sell.
b.	“Gas” fuel and “diesel” cars have the highest sales.
 
 
 
 


 
