LUISS Guido Carli
Artificial Intelligence and Machine Learning

Project on topic
MedCare Wellness Research Center

By Wojciech Augustyniak, E00646; Ignazio Alessandro Rizzini-Bisinelli, 289151; and Angel Mladenov, EO0140

Mentors: Giuseppe F. Italiano; Davide Torre; and Fabio Angeletti

23.12.2023.


Section 1: Introduction

Project Overview

The project involves a detailed analysis of a dataset obtained from a medical center. The primary aim is to explore the relationships between various health indicators, such as hours of sleep, mental health, BMI, and other health conditions, and their impact on an individual's physical health. Using machine learning regression techniques, the study aims to develop a predictive model that can accurately forecast the physical health score of patients based on these indicators.


Section 2: Methods

Data Analysis and Preparation

The dataset, denoted as 'medcenter.csv', comprises a range of health indicators and conditions. Initial analysis involved assessing the dataset's structure, identifying missing values, and determining unique values within each variable. To gain insights into numerical variables, data visualizations like histograms and boxplots were utilized to understand their distributions. Additionally, categorical variables were recognized for further examination in the subsequent stages of analysis.

Feature Engineering

One-hot encoding was employed to convert categorical variables into a format compatible with machine learning models. Particular attention was directed towards feature adjustments due to mislabeling in the domain of Physical Health. Managing outlier values was executed using the Interquartile Range (IQR) method, followed by the normalization of the remaining dataset. Additionally, the dataset underwent a filtration process to eliminate illogical entries, thereby fortifying data integrity. The utilization of correlation analysis proved instrumental in identifying noteworthy features that exert a substantial influence on physical health.




Design decision

Following analysis, it was determined that the nature of the problem aligns with a regression task. Consequently, comprehensive groundwork was laid for data preparation and method selection tailored specifically for this operation.

Initially, linear regression was employed to establish fundamental computations and set a benchmark for subsequent models. Subsequently, a multi-faceted approach was adopted, incorporating Gradient Boosting, Neural Network, and Stacking Regressor techniques. Gradient Boosting, known for its good predictive capabilities through ensemble learning, was selected for its ability to deliver accurate predictions. Neural Networks, better suited for capturing intricate patterns within datasets, were utilized to harness complex data relationships. Additionally, the Stacking Regressor was used to combine diverse models, harnessing their collective strengths to enhance predictive performance specifically in the context of regression problems. This strategic use of multiple techniques aimed to ensure a comprehensive evaluation of predictive methodologies for the given regression task.


Environment and Reproducibility

The data processing and modeling tasks were executed within the Google Colab Python environment, leveraging essential libraries including pandas, NumPy, seaborn, and scikit-learn. These libraries provided support for data manipulation, analysis, visualization, and the implementation of various machine learning algorithms essential for the project's success.



Section 3: Experimental Design

Experiment

Our experimentation involved feature selection processes to identify the optimal set of features to retain within the dataset. After numerous iterations, we determined that a correlation threshold greater than 0.1 yielded the highest R2 scores and minimized Mean Squared Error (MSE) across various feature combinations. While exploring alternative approaches, setting a specific threshold for individual R2 showed comparatively less success when compared to the correlation-based method. Hence, the correlation threshold of 0.1 emerged as the most effective criterion in enhancing predictive accuracy and minimizing errors in our feature selection endeavors.

Model and Validation

We trained and assessed advanced models such as Gradient Boosting, Neural Networks, and Stacking Regressors to ascertain their performance and suitability for the task at hand. To ensure the robustness and generalizability of these models, the dataset was partitioned into distinct training, validation, and test sets, with relative percentages of 80, 10, and 10.


Evaluation Metrics

The assessment of models was conducted using metrics specifically chosen for their efficacy in measuring prediction accuracy and model fit: Mean Squared Error (MSE) and R² score. These metrics provided insightful quantitative measures to gauge the models' performance, allowing for a comprehensive evaluation of their predictive capabilities and how well they capture the variance in the data.

Section 4: Results

Analysis and Interpretation

In-depth scrutiny of model performances showcased the Stacking Regressor as the most effective among the evaluated models, emphasizing the advantages derived from amalgamating divers showed superior performance compared to other models. Figure 1 further illustrates a slightly more favorable outcome for the Stacking Regressor, with respect to R² scores, while Figure 2 shows the Stacking Regressor to have the lowest MSE of the models.

![See 'Figure_1' in 'Images' folder]

Fig.1

![See 'Figure_2' in 'Images' folder]

Fig.2

Section 5: Conclusions

Summary of Findings

This research underlines the promising potential of machine learning within predictive health analytics, emphasizing the significant value derived from the fusion of diverse models to enhance prediction accuracy. The superior performance demonstrated by the Stacking Regressor demonstrates its efficacy in managing intricate and multidimensional healthcare data. This finding accentuates the Stacking Regressor's capability to navigate and derive insights from complex healthcare datasets, thereby showcasing its prominence in advancing predictive modeling within the healthcare domain.

Future Directions

Future studies could delve into expanding the scope by incorporating additional variables, exploring a wider array of machine learning algorithms, and employing more sophisticated feature selection techniques. Additionally, there's an opportunity to validate the model's practical utility and assess its impact on patient outcomes by deploying it within a real-world clinical setting. This practical application would provide valuable insights into the model's effectiveness in a live healthcare environment, potentially enhancing its relevance and usability in improving patient care and outcomes.

