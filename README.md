# Ex02-Outlier

AIM:

    To perform various operations regarding the outliers detection using the given Dataset.
 
ALGORITHM:

You are provided with a csv file(bhp.csv) use that file and removw the outliers using IQR method and get a new dataframe.

Also use zscore method of 3 to remove outliers.

You are given  csv flles(height_weight.csv)

1. Use the IQR method to detect the outliers(WEIGHT) and print them.

2. Use the IQR method to detect the outliers(HEIGHT) and print them.   
    
    
CODE:

```
sns.boxplot(data=df1)

q1=df1.quantile(0.25)
q2=df1.quantile(0.50)
q3=df1.quantile(0.75)
iqr=q3-q1
high=q3+1.5*iqr
low=q1-1.5*iqr

z=np.abs(stats.zscore(df2))
```



OUTPUT:

![Screenshot (230)](https://user-images.githubusercontent.com/119657657/227710110-60b45428-b539-4b54-bd2e-6dc58ef8ff10.png)

![Screenshot (231)](https://user-images.githubusercontent.com/119657657/227710123-3578528f-bfe4-4d5b-b4f5-b5565ed9e8e5.png)

![Screenshot (232)](https://user-images.githubusercontent.com/119657657/227710137-a2fd02f6-5d7b-44cd-8c9f-3ba1c22bb9f6.png)

![Screenshot (233)](https://user-images.githubusercontent.com/119657657/227710146-642b1ced-a25e-4919-824d-1686fffe71a7.png)


RESULTt:

Outliers are detected using the operations(i.e IQR method,,etc). 
