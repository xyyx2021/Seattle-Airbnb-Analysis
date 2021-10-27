# Seattle AirBnB Data analysis

This notebook is written for Udacity Data Science Nano degree project. The objective is to analyze Seattle AirBnB data, including the seasonal trend, pricing analysis and modeling. 

### Table of Contents

- [Installation](#Installation)
- [Project Motivation](#Project-Motivation)
- [Data](#Data)
- [File Descriptions](#File-Descriptions)
- [Answers](#Answers)
- [Blog](#Blog)

### Installation

The following Python libraries (Python version 3.7 or above) installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [seaborn](https://seaborn.pydata.org/)
- [SciPy](https://www.scipy.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

### Project Motivation

For this project, I picked the public dataset of Seattle Airbnb data from Kaggle website: 
Four questions to be answered by analyzing the data are:

1) Which month has the highest/lowest average list price?
2) What are the neighborhoods with highest and lowest price?
3) What are the numerical features strong correlated with price? 
4) How is the predictability of using those features to predict price?


### Data

The data about Airbnb in Seattle can be downloaded from **Kaggle**:

[Seattle Airbnb Open Data](https://www.kaggle.com/airbnb/seattle/data)

It includes three spreadsheets: calendar.csv, listings.csv and reviews.csv.

### File Descriptions

Jupyter Notebook [Seattle_Airbnb_Analysis_Udacity.ipynb] is written to address these questions. 

### Answers

- The listing prices reaches their peak from June to August and are lowest from January to March. The highest listing price is in July, around 152 dollars. The lowest listing price is in January, around 122 dollars.

- The top two neighborhood with highest price are the Southeast Magnolia neighborhood, averaging at 232 dollars and Portage Bay at 228 dollars. The top two neighborhood with lowest price areRainier Beach, averaging at $68 dollars and Olympic Hills averaging at 72 dollars. 

- By illustrating the correlation of all numerical columns in the listing spreadsheet with price column, it is shown the numerical features of bathrooms, beds and bedrooms have strong correlation with the price. Therefore, for the modeling and price prediction, those column will be used.

- Both linear regression and Randomforest regressor were applied to use the numerical features including bathrooms, bedrooms and beds, as input to predict price. The r2 scores on the test data are all below 0.5, indicating that those features alone are not enough to predict price, other information may be needed to improve the predictability, i.e. neighborhood, reviews, etc.

### Blog

[What can we learn about Seattle Airbnb price?](https://medium.com/@xueyang1983?p=2befc3abc46b)
