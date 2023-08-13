# Lead-Score Case Study
## Problem Statement

- Develop a lead scoring model that takes into account various factors to predict the conversion probability for each lead.
- Assign lead scores to each lead based on the model's predictions.
- Identify the leads with the highest scores as the 'Hot Leads' with the greatest potential for conversion.

By implementing this predictive model, X Education aims to optimize their lead conversion process, focus their sales efforts on the most promising leads, and ultimately achieve the target conversion rate of 80%.

Steps Followed
----------------------------------------------------------------------------------------------------------------------------------------------------

- Dataset Reading
- Data Understanding using info, describe, null value counts, unique value counts, value distribution of each columns.
- Exploratory data analysis - this include Univariate analysis and bivariate analysis.
- Data Preperation - Creating dummy variables
- Splitting the data in Test and Train.
- Feature Scalaing using MinMaxScalar - As no outliers has been found in the numerical columns
- Feature Selection using RFE
- Model Building
- Confusion Matrix
- AUR-ROC Curve
- Precision Recall 
- Predicition on Test Set

Conclusion
---------------------------------------------------------------------------------------------------------------------------------------------------
#### Model Evaluations 
The evaluation of the model's performance provides key insights into its predictive capabilities for both the train and test datasets. The metrics employed for assessment encompass accuracy, specificity, and sensitivity, each contributing to a comprehensive understanding of the model's effectiveness.

##### Train Data Evaluation:

**Accuracy:** The model demonstrates a commendable accuracy rate of 79.78% on the train dataset. This metric gauges the overall correctness of the model's predictions, highlighting its proficiency in classifying instances correctly.

**Specificity:** A specificity rate of 81.43% is observed for the train dataset. This metric elucidates the model's aptitude in accurately identifying negative instances, contributing to its ability to correctly distinguish non-target outcomes.

**Sensitivity:** The model exhibits a sensitivity rate of 78.77% on the train dataset. This metric signifies the model's capacity to effectively identify positive instances, showcasing its prowess in correctly recognizing target outcomes.

##### Test Data Evaluation:

**Accuracy:** Similarly, the model achieves an accuracy rate of 79.82% on the test dataset. This reaffirms the model's consistent predictive performance on previously unseen data.

**Specificity:** Notably, the specificity rate for the test dataset rises to 82.62%. This indicates the model's ability to correctly identify negative instances, showcasing its robustness in handling non-target outcomes.

**Sensitivity:** The sensitivity rate for the test dataset stands at 78.09%. This underscores the model's capability to accurately identify positive instances, further affirming its proficiency in recognizing target outcomes.

Collectively, these evaluation metrics furnish a comprehensive depiction of the model's strengths and areas of excellence. The balanced assessment of accuracy, specificity, and sensitivity contributes to a well-rounded evaluation of the model's predictive prowess, both on the train and test datasets.

#### Feature Importance Analysis and Variable Influence

The key variables that exerted the most significant influence on the outcome were identified through their corresponding coefficient values within the logistic regression model. These coefficients signify the strength and direction of the relationship between each predictor variable and the likelihood of the target event occurring.

##### Positive Coefficient Effects:

- Total Visits: The total number of visits to the website exhibited a positive coefficient, suggesting that an increase in the count of visits was associated with a higher probability of the target event.

- Total Time Spent on Website: The duration of time spent by individuals on the website also displayed a positive coefficient. This indicates that a longer engagement period with the website positively influenced the likelihood of the target event.

- Working Professional: The status of being a working professional yielded a positive coefficient, indicating that individuals with this designation were more likely to experience the target event.

- Lead Source - Welingak Website: The origin of leads from the "Welingak" website demonstrated a positive coefficient, suggesting that leads originating from this source were more likely to result in the target event.

##### Negative Coefficient Effects:

- Lead Search (Google, Organic Search, Referral Sites): The inclusion of variables related to lead searches, including those originating from Google, organic search, and referral sites, displayed negative coefficients. This suggests that leads from these search sources were associated with a reduced likelihood of the target event.

- Last Activity (Converted to Leads, Olark Chat Conversation, Email Bounced): Certain last activities, specifically those denoting conversion to leads, engagement through Olark chat conversations, and instances of email bounces, exhibited negative coefficients. This implies that leads with these last activities were less likely to result in the target event.


In summary, the logistic regression analysis revealed distinctive variables with both positive and negative coefficients, signifying their differential impact on the probability of the target event occurrence. These insights provide valuable guidance for understanding and potentially influencing the factors contributing to the target outcome.


##### Hot Leads Selection

The distribution of leads across varying lead scores underscores the significance of lead scoring in discerning potential high-value prospects. Notably, the analysis reveals the following counts for leads with lead scores surpassing specific thresholds:

- Lead Scores > 90: The dataset encompasses a robust count of 283 leads whose lead scores exceed the threshold of 90. This subset is indicative of leads that exhibit exceptional attributes aligning with a heightened propensity for conversion.

- Lead Scores > 80: The dataset further includes a substantial cohort of 477 leads that possess lead scores surpassing 80. These leads demonstrate characteristics that position them as promising candidates with a strong likelihood of converting into valuable clientele.

- Lead Scores > 70: Within the dataset, a significant assembly of 602 leads showcases lead scores surpassing 70. This subset signifies a noteworthy aggregation of leads exhibiting qualities suggestive of an increased potential for conversion.

- Lead Scores > 60: Additionally, the analysis identifies a substantial grouping of 698 leads with lead scores exceeding 60. This subset encompasses leads that bear promising attributes, signifying a favorable outlook for eventual conversion.

Collectively, these observations underscore the utility of lead scoring in segregating leads into distinct strata, enabling targeted engagement strategies based on their respective lead scores. Such insights empower effective resource allocation and tailored interactions to optimize lead conversion rates.