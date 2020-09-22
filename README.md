<p align="center">
   <img src=https://github.com/yeagercmbpd/DATA602_HW1_AutoPrices/blob/master/Images/Banner2.png />
<div align="center">
   <figcaption></figcaption>
</div>
</p>

                                              **Anticipating Automotive Sales Prices for Inventory Aquisition**

### Overview and Project Goals

Obtaining the proper vehicles to maximize profit in the used auto market can prove difficult. We have obtained a dataset which includes the used vehicle values from all Craigslist used car listings during the current year, in an attempt to identify those features which have the greatest impact on automotive resale value. In addition, the data was fitted to a linear regression model to allow for pricing predicitive capabilities for possible purchases.
---
### Repository Navigation
<pre>
Data Cleanup  : <a href=https://github.com/yeagercmbpd/DATA602_HW1_AutoPrices/blob/master/Notebooks/Kaggle_CLAutos_DataCleanup.ipynb>Data Preprocessing Notebook </a>
Model Building: <a href=https://github.com/yeagercmbpd/DATA602_HW1_AutoPrices/blob/master/Notebooks/Linear_Regression_Model.ipynb>Building the Model Notebook</a>
Visualizations: <a href=https://github.com/yeagercmbpd/DATA602_HW1_AutoPrices/blob/master/Notebooks/Further%20Business%20Problem%20Visualizations.ipynb>Visualizations Notebook</a>
</pre>
---
### ReadME Navigation

[Data](https://github.com/yeagercmbpd/DATA602_HW1_AutoPrices/#data) -
[Model](https://github.com/a-woodbury/A-House-with-a-View#model) -
[Results](https://github.com/a-woodbury/A-House-with-a-View#results) - 
[Recommendations](https://github.com/a-woodbury/A-House-with-a-View#recommendations) - 
[Future](https://github.com/a-woodbury/A-House-with-a-View#future) - 
[Project Info](https://github.com/a-woodbury/A-House-with-a-View#project-info) -

---

## The Data
This dataset used in this analysis was located on Kaggle [Used Cars Dataset: Vehicles listings from Craigslist.org](https://www.kaggle.com/austinreese/craigslist-carstrucks-data). The data is made up of all content, as scraped from the CraigsList used vehicle listing section. It was last updated in January 2020, and consists of 509,577 records, with 25 features. Of these, our study uses only those from our sales region (MD, VA, PA, and WV), as well as those records which are the most robust in terms of feature content; resulting in a filtered and formatted dataset of roughly 10,000 records. 

---

## Features and Limitations 
Automotive sales data (new or used) is a commodity which is gaurded tightly by its owners. Other large websites, such as Autotrader or Cars.com, as well as major auto manufacturers do not make thier data widely (or cheaply) available. Additionaly, pages like autotrader have provisions against scraping and no open API. Resources like Craigslist, however, provide a glimpse into the state of the used vehicle market. The variables we were able to clean and utilize from this dataset are as follows:
   Continuous: Price (target), Age, and Vehicle milage.
   Categorical: Manufacturer, Model, Condition, Engine cylinders, Vehicle type (ie truck, car, van), and Transmission type.
   
This being an open source dataset does have its drawbacks. Some of the data is the subjective opinion of the listing individual, overall vehicle condition for example. In addition, some of the fields from above are open text and thus standardization for something like vehicle model is nearly impossible. a variation of over 2500 entries were found in just our filtered dataset of 10,000 records.

---

## Summary Results

Explained variance: 65%

Throughout the analysis it became clear that the simple variables of vehicle age and milage are always going to be the safest way to get a return on investment. They were correlated the most strongly and consistently, regardless of other factors at play. Additionally, however, an R2 result of greater than 50% could not be achieved without the additional information provided by the manufacturer, engine cylinders, vehicle type, and transmission features. Unfortunately, condition and model returned as not playing a statistically signifigant role in model output. We theorize this is due to the bias of the seller as to condition and inconsistency in model accuracy input in the dataset.

---

## Packages and Credits
<pre>
By : <a href=https://github.com/yeagercmbpd>Christopher Yeager</a>
</pre>

<pre>
Languages    : Python
Tools/IDE    : Jupyter
Libraries    : pandas, numpy, matplotlib, statsmodels, sklearn, seaborn
</pre>
