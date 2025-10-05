# Game-Winner-Prediction

- **Dataset Link** : https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1012-GameWinnerPred.zip


## 🎯 Project Objective

* Goal: Predict the likelihood of winning a PUBG (PlayerUnknown's Battlegrounds) game based on player 			statistics.

* Dataset: Large dataset with 4,446,966 entries and 29 columns, containing information on player behavior, 		match types, and outcomes.

## 📚 Data Preprocessing & Handling
* Initial Checks:
          Checked for duplicates and removed them.
* Handled missing values:
          Dropped rows with missing winPlacePerc values.
* Label Encoding applied to:
          matchType, Id, groupId, and matchId.
* Feature Scaling:
          Applied StandardScaler to normalize numerical features.

## 📊 Exploratory Data Analysis (EDA)
	
* Univariate & Bivariate Analysis:
    * Analyzed distributions and relationships between key features.
		Visualized match types, damage dealt, kills, and more.
* Outlier Handling:
		 Identified and addressed potential outliers using boxplots and histograms.

## 🧠 Model Building & Evaluation
	
  * Models Evaluated:
    
	  * Linear Regression
		
    * Decision Tree Regressor
		
    * Gradient Boosting Regressor
		
    * XGBoost Regressor
		
    * AdaBoost Regressor
	
  * Feature Importance:
    
	* XGBoost feature importance revealed that key variables like killPlace, killPoints, and damageDealt 		had the most impact on predicting the outcome.

## 📈 Model Performance Summary
	
  * Best Performing Model: XGBoost Regressor
		
    * R² Score: 0.93
		
    * Mean Squared Error: 0.0068
		
    * Mean Absolute Error: 0.0068
	
  * Overall Model Comparison:
	
    * Models performed well with R² scores ranging from 0.82 to 0.93.

## 📊 Model Comparison Report
```
Model	        			  R² Score
Linear Regression	  	       0.85
Decision Tree Regressor		   0.85
Gradient Boosting Regressor	   0.89
XGBoost Regressor		       0.93
AdaBoost Regressor		       0.82
```
## ⚡ Challenges Faced
	
  * High Dimensional Data:
		 Large dataset required efficient handling and scaling for optimal model performance.
	
  * Outliers & Data Imbalance:
		 Addressed outliers and ensured balanced feature distribution.

## ✅ Conclusion
	
* XGBoost Regressor achieved the highest R² score of 0.93, indicating a very high prediction accuracy.

* Feature importance analysis highlighted that kill-related features were the most predictive.
