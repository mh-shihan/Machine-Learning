# Handling Missing Values in Data Analysis
![alt text](image.png)


## Complete Case Analysis(CCA)
Complete Case Analysis also called "list-wise deletion" of  cases, consists in discading oversvation(row) where values in any variables are missing. 

Complete Case Analysis means literally analyzing only those observations for which there is information in all of the variables(col) in the dataset. 

## When to apply CCA
- When the missing values are missing completely at random (MCAR).
- When the proportion of missing values is small. Generally less than 5% of the total data.

## Advantages of CCA
- It is simple to implement and understand.
- Easy to implement as no data manipulation is required.
- Preserve variable distribution as it does not impute any values.

## Disadvantages of CCA
- It can exclude a large portion of the dataset, leading to loss of information and reduced statistical power.
- It can lead to biased estimates if the missing data is not MCAR (Missing Completely At Random).
