# IBM-HR-Attrition  
**Introduction**  
In this project, I perform a quick analysis of the IBM HR attrition data to explore valuable insights into the reasons behind employee attrition. Additionally, I construct a machine learning model to predict employee attrition, achieving an accuracy score of nearly 0.9, which demonstrates strong predictive capabilities.

**Insights**
- As income increases, attrition decreases.  
- Attrition is much less in divorced men.  
- Attrition is highest for employees in level 1 jobs.  
- Attrition is high among men in sales expert roles.  
- Women in managerial, research director, and laboratory technician roles have very low attrition.  
- Attrition is highest for both men and women from 18 to 35 years of age, then gradually decreases.  
- Attrition is higher for employees who usually travel than others, and this rate is higher for women than for men.

**Machine Learning model**
*Problem:* Our data faces an imbalance problem, as the number of employees with attrition is much smaller than those without. In standard machine learning algorithms like Decision Trees and Logistic Regression, this imbalance can lead to a bias toward the majority class, causing the minority class to be overlooked. As a result, these models often predict only the majority class, leading to a significant misclassification of the minority class compared to the majority class.  
  
*SMOTE:* To address this imbalance, we will use the SMOTE method, one of the most widely used oversampling techniques. SMOTE balances class distribution by generating new instances of the minority class through interpolation rather than simple replication. After oversampling, the data is restructured, allowing for the application of various classification models on the balanced dataset.  

I have constructed two machine learning models for attrition prediction: Logistic Regression and Random Forest Classifier. Both models perform excellently on the data; however, the Random Forest Classifier outperforms the Logistic Regression model, achieving a higher accuracy score (0.90 - Random Forest > 0.83 - Logistic Regression). For a detailed analysis, please review my Python file in this GitHub repository.

**Recommendations**  
Enhance Job Satisfaction:  
-  Improve employee benefits and support, especially in departments with low satisfaction.  
-  Conduct regular surveys to understand and address employee needs.

Manage Work Hours:  
-  Reduce overtime, especially in high attrition departments like Research & Development.  
-  Implement flexible working hours and remote work options.  

Increase Salaries and Benefits:  
-  Reevaluate salary and benefits policies to ensure competitiveness.  
-  Offer bonuses for high performers to retain talent.  

Improve Working Conditions:  
-  Support employees who travel frequently with rest periods and work-life balance measures.  
 
Review Promotion Policies:  
-  Ensure promotion opportunities are fair and transparent.  
-  Adjust promotion policies to align with employee expectations and reduce perceived inequities.  


