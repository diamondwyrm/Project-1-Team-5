# Analysis Write Up

## Demographics
<Kent's analysis here>

## Severe Weather Events
<Laura's analysis here>

## Rental Market
<Tim's analysis here>

## Housing Layouts 
In an effort to gain experience using a very large and very dirty dataset for this project, I selected a dataset that was provided by Zillow in a $1M machine learning contest to improve the Zillow "Zestimate" algorithm.  The datasat contained housing amenities and information for nearly 3 million houses in Orange, Ventura, and LA counties in 2016.  

For the project, I spent a lot of time doing exploratory analysis on the contents of the dataset and determined areas that could be cleaned.  For example, I filtered out the datasets that contained either zero bedrooms or bathrooms, since those numbers were causing alot of skewed results.  Next, I created a box plot to determine the layout outliers (I'm sure there ARE 15 bedroom houses in SoCal, but for this analysis, I felt it was better to examine non-outliers).  Due to the volume of data provided, I decided to focus on the number of bedrooms and bathrooms in a house.

As expected, the layout of a house does impact the value of the house.  Specifically, as the number of bedrooms increases, the value of the house increaes from $56k to $137k. We can take this a step further by creating a heatmap of the layout of the house and look at the number of bedrooms and bathrooms.  The general trend that we observe is that as the number of bathrooms increase, so does the house value.  Interestingly, the most valuable houses shown in the heatmap are those with the most bathrooms and less bedrooms.  This prompted me to look at the sample size of each layout.  As we can see by plotting the total percentage of each layout on a heatmap, the smaller sample size of 1 bedroom, 4 bathroom houses is likely contributing to the higher overall prices.  