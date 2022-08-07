# dont-overbid
build a model for house price estimation

Several years ago, we started thinking of purchasing a house for my family. To make sure we don’t end up overbidding, I needed to know what price we should make our offer at. Of course, there are many websites that I can go to, but often their ranges were too big to make a good estimation. I decided to try on my new knowledge and produce the estimation myself! 
The good model for this project would be linear regression. So I decided to use the scikit library because it has a range of stable regression models, not to mention easy-to-use data split functions. Following was my process:      
Requirement: Python 3.8, sklearn, numpy, pandas, matplot, seaborn, jupyter lab   
Collect data: I collected the data right from Redfin. They provide a nice feature of data export for the public. I narrowed it down to several cities and applied some conditions I want, such as single home, at least 3 bedrooms
Load and preprocess: 
Make sure to take a look at the data first before loading. 
Go through the data for structure, # of observations, etc. 
Check the features and drop any if needed. 
Check for any missing values, and decide what to do with them. (drop or fill)
Check if the data type is correct and convert if needed. 
Check for categorical values and apply one-hot encoding. 
See if I need to create my own features: I tried bed/bath room ratio. They have positive correlation, according to my domain knowledge. 
Split training and testing 
Model selection - linear regression seems most appropriate
Fit the training to the model 
Apply prediction on testing. Find the stats such as pearsonr and residuals 
Visualize the residuals (differential between actual and prediction)
Try the house I consider to this model and see the predicted price
