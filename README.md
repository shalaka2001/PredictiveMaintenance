### Project Title: Predictive Maintenance of Smart Grids using AI/ML

**Shalaka Tarkar**

#### Executive summary: 
A Smart Grid is an electricity network that use digital technologies, sensors and software to monitor and manage the transport of electricity from all generation sources (renewable, non-renewable and DERs(Distributed Energy Resources) to meet the varying electricity demands of end users. Smart grids co-ordinate the needs and capabilities of all generators, grid operators, end users and electricity market stakeholders to operate all parts of the system as efficiently as possible, minimising costs and environmental impacts while maximising system reliability, resilience, flexibility and stability. It is an IoT-based application and uses real-time data on energy consumption to balance electricity supply and demand. 

Surge in electricity demands(say heatwave or extreme cold temperatures), unbalanced loads or incorrect demand forecasting can cause electricity Overloads in the grid and result in blackouts or brownouts, voltage fluctuations. Transformers can fail due to overloads, lightning, short circuits, poor maintenance causing complete power loss, fire or explosions, high replacement costs and long repair times.

#### Rationale
This question holds significant importance in today’s digital era, where a reliable electricity supply is essential. Predictive maintenance should become a standard practice, enabling utility companies to take timely corrective actions. By leveraging alerts generated by predictive models, operators can proactively adjust load distribution or schedule maintenance activities. This approach helps prevent unexpected outages, reduces repair costs, and minimizes inconvenience for utility customers


#### Research Question
##### Given current electric smart grid readings, can I predict if system would experience a failure in the next time interval

#### Data Sources
##### (https://www.kaggle.com/datasets/ziya07/smart-grid-real-time-load-monitoring-dataset)

#### Methodology
##### I will be using the following CRISP-DM methodology
- Data Analysis of the above data to determine the parameters captured. Understand what parameters are actually required and how can I use this in actual setting
- Data Cleansing and Standrdization, understanding the features and feature engineering
- As the parameters were concise, I did not use any PCA analysis
- Classification Model generation using GridSearchCV and Logistic Regression, Random Forest, KNN, SVM, Decision Tree and Neural networks algorithms. Evaluating the Grid Search hyperparameters to determine the best model.

#### Results
As the data is highly imbalanced, amongst all the algorithms that I evaluated - 
1. SVM had the best balance of accuracy 41% and highest "Yes" class recall 61%, which means that it could identify positive overload and fault scenarios better than other models.
2. Neural Networks with Keras Classifier, 3 Dense layers and metrics of "F1" yielded 55% recall and 45% accuracy - by far the best amongst all the models I trained.

#### Next steps
For this model to be used in an actual production setting, I will need to demo it to my leadership to show the potential. The model needs to be deployed and an API end point needs to be exposed to generate the output based on the readings input. As the electricity grid changes with additional components added/removed, actual data from the field needs to be used continuously to train the model (may be nightly) to make it more precise to detect the Overload or Fault scenarios.

#### Outline of project

- https://github.com/shalaka2001/PredictiveMaintenance/blob/main/PredictiveMaintenance.ipynb


##### Contact and Further Information
Shalaka Tarkar
Email: shalaka_ntarkar@yahoo.com
