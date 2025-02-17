# PRODIGY_DS_02_V2
Exploratory Data Analysis </br>
I usde a data set from Kaggle AER_credit_card_data.csv </br>
</br>
</br>
</br>
**What is exploratory data analysis?** </br>
Exploratory data analysis (EDA) is a technique that data professionals can use to understand a dataset before they start to model it. Some people refer to EDA as data exploration. The goal of conducting EDA is to determine the characteristics of the dataset. Conducting EDA can help data analysts make predictions and assumptions about data. Often, EDA involves data visualization, including creating graphs like histograms, scatter plots and box plots </br>
</br>
</br>
</br>
Before you begin exploratory data analysis, it's important to understand a few key terms:
## Value: 
A data value is a piece of information, such as a number or a date.</br>
## Variable: 
A data variable is a characteristic that you can measure, such as weight or income.</br>
## Distribution: 
The distribution of a dataset is how the dataset is spread out. You can visualize a dataset's distribution by observing its shape on a graph.</br>
## Outlier:
An outlier is a data value that is significantly different, including much higher or lower, from the rest of a dataset.</br>
## Data model: 
A data model is a method of organizing data and relationships between values in a dataset.</br>
</br>
</br>
</br>
Potential issues:

- We'll want to convert income into the same units as expenditure.</br>
- Both dependents and age are flagged as problematic so we should take special note of those columns.</br>
- months might be more useful if we converted it to the same units as age.</br>


first I aplaoded the data set and creat a panda data frame, then I showed few rows of it, I missed around with some pandas function like isna(), shap, describe(), dtypes() ans so on then I converted the yes or no of the column card into 0 and 1 using the function map 

</br>
</br>
</br>

- The binary value columns do need to be converted to True/False.</br>
- 50% of the population falls within a 15 year age range. I would have expected a random sample of credit card holders to be more uniformly distributed across the adult age range. If possible, it would be helpful to understand the original sampling process.</br>
- majorcards appears to be a boolean rather than a count, contrary to the manual.</br>
- The maximum value for Active is suprisingly high, but theoretically possible. A domain expert might be able to shed light on this.</br>
- The share column is supposed to equal the ratio of monthly credit card expenditure to yearly income. Given that the minimum expenditure is zero and the minimum share is not, there's either an error in the manual or with the calculation of share.</br>
