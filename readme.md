**Simple Linear Regression For Real State value Prediction.** <br /> 
Linear regression model is used to find approximate relationship between independent and dependent variable which wan be represented by a straight line. <br /> 
**Libraries requried:** Panda, Numpy and Matplotlib <br /> 

**Explanation** <br /> 

The dependent data are 'X1 house age', 'X2 distance to the nearest MRT station', 'X3 no of convenience stores', 'X4 latitude', 'X5 longitude', and the independent data is 'Y house price of unit area.'Dependent data has been used for training, and  X is the variable taken to declare training data. Independent data is used for testing, and Y is taken as a variable for the declaration of testing data.As there are 5 data for training each data are trained separately by creating data rame under the variable X as shown  <br /> 
X=pd.DataFrame(data, columns=['X1 house age']).values  <br /> 
X=pd.DataFrame(data, columns=['X2 distance to the nearest MRT station']).values <br /> 
X=pd.DataFrame(data, columns=['X3 no of convenience stores']).values  <br /> 
X=pd.DataFrame(data, columns=['X4 latitude']).values, X=pd.DataFrame(data, columns=['X5 longitude']).values <br /> 

And as there is one independent variable data frame is created as Y = pd.DataFrame(data, columns=['Y house price of unit area']).values <br /> 

For each training set mean was evaluated for each dependent variable, and the mean was estimated for the dependent variable after finding mean b1 and bo were calculated. then max and min value of the training set was evaluated, then x is a variable declared where linspace was 
considered using min and max value, and y was calculated using **y = b0 + b1 * x**, then the regression line was drawn using x and y, and the scatter plot was drawn using X, Y for each dependent value separately. At the end error was calculated between the actual value(Y) and predicted value(y) for all the five dependent variables separately. Then all error average is computed using mean square error separately.
