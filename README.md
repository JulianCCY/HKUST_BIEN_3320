# HKUST BIEN 3320 Data Science for Biology and Medicine Project (Correlation between Risk Factors and Coronary Heart Disease)


<p align="center">
<img width="400" height="300" src="https://media.tenor.com/esJfyI68v6oAAAAM/sanford-fred.gif"/>
</p align="center">


The reason our topic is worth investigating and why we are interested in it is because chronic heart diseases have been a prominent issue and CHD in particular, is responsible for around 37,000 deaths in 2021. It is also the third most common cause of death in Hong Kong. Lifestyle diseases share risk factors similar to prolonged exposure to modifiable lifestyle behaviors like smoking, unhealthy diet, and physical inactivity, and they result in the development of chronic diseases, specifically heart disease. The course of the disease in patients with chronic heart diseases is different. Complications can occur to different extent that may lead to worsening of the disease and even death. Even an experienced specialist can not always foresee the development of these complications.

## Abstract
The topic for investigation is the correlation between risk factors and coronary heart disease (CHD), where we look into the association of CHD and aspects ranging from daily life practices like doing sports, to other further complications like stroke. For the results, we have concluded that there are a few risk factors that are significantly related to the prevalence rate of CHD; the correlation of each risk factor is visualized by a scatter plot. Stroke and diabetes were also investigated as complications of CHD, where they also share similar association patterns with certain risk factors as that of CHD. The extent of correlation is represented by a correlation matrix of those risk factors and CHD, stroke, and diabetes. The dataset we adopted is a survey with around 250,000 responses, which has broad coverage. Accuracy prediction of how comprehensively the results predict the prevalence rate of CHD is at 90.67%. 

## Introduction
Chronic heart diseases have been a prominent issue in society and CHD in particular, is responsible for around 37,000 deaths in 2021 (HealthHK, 2021). It is also the third most common cause of death in Hong Kong (Statista, 2020). Lifestyle diseases share risk factors similar to prolonged exposure to modifiable lifestyle behaviours like smoking, unhealthy diet, and physical inactivity, and they result in the development of chronic diseases, specifically heart disease. The course of the disease in patients with chronic heart disease is different. Complications can occur to different extents that may lead to worsening of the disease and even death. Even an experienced specialist can not always foresee the development of these complications (Golovenkin, S.E. et al., 2020). 

Leading questions surrounding the main topic:
- How different risk factors affect the prevalence rate of CHD?
- Which factors are positively or negatively correlated with CHD?
- Do other common complications share any similarities or differences with CHD in the correlations between different risk factors? 


## Methodology
Dataset from the Behavioural Risk Factor Surveillance System (BRFSS), which is an annual survey conducted by the Centers for Disease Control and Prevention (CDC), is used for our investigation. The survey results were uploaded onto the public accessible website Kaggle by author Alex Teboul (Teboul, A., 2022). The survey collects responses related to risk factors such as personal health status, living habits and anamnesis. JupyterLab 3.5.3 is used to perform all data processing in our project. Data preprocessing and cleaning, including dropping missing values, filtering unwanted outliers, and scaling numeric features is first done in order to lead to a more conclusive and accurate decision. We excluded any survey responses which are incomplete and dropped risk factors that are insignificant in correlation representation. 

To preliminarily view the relationship between CHD and different risk factors, several graphs of the prevalence rate of CHD against different age levels were plotted. Each graph involves a change in one risk factor, and the correlation changes due to the variation in the risk factors can be observed by comparing the difference in the trend of the colour dots. The factors we investigated include body mass index (BMI), walking ability, blood pressure, blood cholesterol level, smoking habit, physical activity level, vegetable and fruit consumption. Afterwards, the correlation significance between CHD and different risk factors can be visualized by the graphs.

In view of the problem that the scatter plots mentioned above may be affected by the correlation among the risk factors themselves, pair plots were made to further investigate the strength of correlations between CHD and a particular risk factor when other factors also vary. The pair plots show the general correlation between any two risk factors, and the difference of these correlations when CHD exists or does not exist, represented by different colours of dots. The strength of the correlation between CHD and one risk factor can be observed by viewing the separation of the colour dots across all the pair plots related to the target risk factor. 

Correlation analysis is derived to investigate whether other common complications, such as stroke and diabetes, share similarity or difference with CHD in the correlation with different risk factors. Due to the nonlinearity of the relationships, Spearman’s Correlation is used to seek for the interdependence of the risk factors and the diseases. Correlation matrices of different diseases were generated using the calculated Spearman’s Correlations, and the similarity and difference can be obtained by comparing the three matrices. 

Machine learning algorithms were also applied to make predictions. The goal is to predict heart disease or attack based on the observation or features from the dataset. We used python, pandas and scikit-learn libraries to perform accuracy prediction. Several machine learning algorithms such as Logistic Regression, K-Nearest Neighbors, Random Forest, XGBoost,  AdaBoost, Gradient Boosting were used to predict CHD. Each algorithm is trained and evaluated by Log Loss and F1 Score.

## Conclusion
In conclusion, different risk factors do have an effect on the prevalence rate of coronary heart disease, with walking difficulty being most positively correlated and physical health being the most negatively associated.  Furthermore, stroke and diabetes share a similar correlation as CHD for a few of the risk factors, namely difficulty in walking, physical health and vegetable consumption. Machine learning algorithms applied to the dataset were able to return accurate predictions. The project can be expanded in the future by incorporating additional medical attributes, exploring different algorithms, or applying them to different datasets. 




## Appendix
For detailed information about the appendix, please refer to [project report 7.Appendix](https://github.com/JulianCCY/HKUST_BIEN_3320/blob/main/documentation/BIEN3320%20Report%20-%20Group%20N3.pdf).

## License
[AGPL-3.0 License](https://github.com/JulianCCY/HKUST_BIEN_3320/blob/main/LICENSE)

## Contributors
[Chan Chung Yin](https://github.com/JulianCCY): Desktop research, data visualization(correlation matrix) and Machine Learning Prediction

Au Yat Sin Candice: Desktop research, data cleaning and processing,

Chui Yuen Tsun: Desktop research, data visualization(scatter plot & pairplot)
