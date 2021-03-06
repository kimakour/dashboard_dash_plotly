# An example of a dashboard built by Dash from Plotly for this fish dataset.
the data set can be found here : https://www.kaggle.com/likhitsudha/fishweights 
### Demo of the Dash app
![Alt Text](https://github.com/kimakour/dashboard_dash_plotly/blob/main/images/dash_demo.gif)

It is divided into three parts :
### Basic visualizations for the features
- Histogram plot
- Scatter plot with possibility of showing the distribution of each feature
- Density heatmap 
![alt text](https://github.com/kimakour/dashboard_dash_plotly/blob/main/images/dash_1.png)

### Model performance
- Table containing basic regression metrics 
- Pie chart for thresholds of the absolute error 
- Scatter plot for the error according to the prediction 
- REC curve and AUC score 
![alt text](https://github.com/kimakour/dashboard_dash_plotly/blob/main/images/dash_2.png)

N.B : there was no feature engineering, hyper-parameter optimization or other modeling step to make the best out of the model.
Furthermore, we have used a linear regression model.
The aim of this dashboard isn't to reach the best performances. It is more like a tutorial for using Dash from Plotly.

### Model interpretability using SHAP values 
- Feature importance using the mean of absolute values of SHAP values for each feature
- SHAP dependence plot 
- Individual explanation 

![alt text](https://github.com/kimakour/dashboard_dash_plotly/blob/main/images/dash_3.png)

N.B : Since we have used in the model performance a linear regression, there is no need to create an interpretability step for the model.
Looking at the parameters is enough.
For the sake of demonstration, we will use in this part a Gradient boosted trees and we will explain it with a Tree explainer from SHAP.
For more info about SHAP values look at : https://papers.nips.cc/paper/7062-a-unified-approach-to-interpreting-model-predictions.pdf 

Please feel free to contact me to enhance the design or add/modify the functions that were implemented in this app.
