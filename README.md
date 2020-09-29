# understanding-the-viewers

### Hi 👋
Let me just explain the objective/problem statement quickly before we hop on to the approach.
Here we are given some data of a newly launched show on some online platform for example Netflix or Amazon. So the marketing team of the company wants to know why the number of viewers are decreasing or what features, or in lay man language what causing the disinterest of viewers in the show.

Now this can happen because of various reasons 🤔:
  1. Decline in number of people coming to platform this can be due to competition or some free sources
  2. Decrease in marketing
  3. Special holidays and people went for vacation
  4. Competition shows like Cricket/IPL 
  5. Viewers don't like the new plot twist

From above mentioned reasons only a few can be managed by the marketing team or show editors. But those few can have a great impact.
So with our data set we will try to figure out which feature have significant impact on the Viewers(which is our target).

### 👉 Features' description:
  1. Date: This column has the date from the start and end of the show.
  2. Views_show: This column has day wise number of views of the show and this is our target variable 
  3. Visitors:   This column has the number of visitors for that show.
  4. Views_platform: This column has the total number of viewers on the platform for that day.
  5. Ad_impression: This is related to marketing, where user clicks on some link and lands on the show page.
  6. Cricket_match_india: This column tells if there was any cricket match on that day or not. For country like India where cricket is a second religion and this alone can have huge impact on shows.
  7. Character_A: This column represents the presence of some main/lovable character, basically a plot twist in case this character dies.
  
  Here to understand 😎 the impact of the features, we will use OLS and statistics for their significance.
  
  OLS stands for Ordinary Least Squares. Well accoding to wikipedia OLS is a type of linear least squares method for estimating the unknown parameters in a linear regression model.
  And when we use OLS's summary in our code we will mainly look for two things R-Squared and p>|t| values.
  
  R-Squared: Also known as Coefficient of Determination. It is the proportion of the variance in the dependent variable that is predictable from the independent variable(s). Basically it is the goodness of fit measure for linear regression. It's value ranges from 0 to 1. For good model it should be closer to 1.
  
  P-value: If the value is less than 0.05 then the variable is significant, otherwise it is not. For indepth understanding of this. Please read about Hypothesis testing and significance value.
  
# About Models:
We will test different models with different columns so that we can get an idea which features have impact on Target variable.
We drive extra features from existing features just to gain better understanding.
Like weekends and week days. People tends to binge watch on weekends.

In every model we reject the features which have p value greater than 0.05 or if that feature is not playing any role in increasing the R-Squared.




  


