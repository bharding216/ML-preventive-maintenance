# ML Model to Predict Pump Station Failure

## Background and Motivation
A town's pump station has equipment that is failing. When equipment fails, the entire process comes to a halt and the failed equipment needs to be taken out of service and fixed before startup can begin. When the process unexpectedly fails, it takes longer for maintenance personnel to address the problem than if they proactively checked the equipment.

Therefore, in order to minimize the overall process downtime, the maintenance supervisor would like to proactively address system issues before they bring down the entire pump station.

Machine learning is a perfect solution for this problem because:
<ol>
  <li>There are complex patterns and non-linear relationships,</li>
  <li>There is a large amount of labeled data,</li>
  <li>There is high dimensionality,</li>
  <li>The environment is susceptible to changes over time, and</li>
  <li>This is a classification task.</li>
</ol>

Overall steps:
<ul>
<li>Data Engineering & Exploratory Data Analysis</li>
  <ul>
    <li>Sanitize and Prepare the Data for Modeling</li>
    <li>Perform Feature Engineering</li>
    <li>Use Machine Learning to impute missing data</li>
    <li>Analyze and Visualize for Machine Learning</li>
  </ul>
<li>Modeling</li>
  <ul>
    <li>Model Selection</li>
    <li>Training</li>
    <li>Hyperparameter Optimization</li>
    <li>ML Model Evaluation</li>
  </ul>  
</ul>

## Result and Conclusion
Using a tuned XGBoost model, we correctly identified all instances of an equipment malfunction event. We do this at the expenses of incorrectly labeling 7 instances as indicative of an equipment malfunction event.

This is acceptable for this scenario, since the downside of checking the equipment when it is not actually faulty is less impactful than not identifying faulty equipment when it is truly faulty (approaching a breaking point). 
