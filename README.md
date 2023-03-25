# Ex02-Outlier

You are given bhp.csv which contains property prices in the city of banglore, India. You need to examine price_per_sqft column and do following,

(1) Remove outliers using IQR 

(2) After removing outliers in step 1, you get a new dataframe.

(3) use zscore of 3 to remove outliers. This is quite similar to IQR and you will get exact same result

(4) for the data set height_weight.csv find the following

    (i) Using IQR detect weight outliers and print them

    (ii) Using IQR, detect height outliers and print them
    
CODE:

sns.boxplot(data=df1)

q1=df1.quantile(0.25)
q2=df1.quantile(0.50)
q3=df1.quantile(0.75)
iqr=q3-q1
high=q3+1.5*iqr
low=q1-1.5*iqr

z=np.abs(stats.zscore(df2))



OUTPUT:

![Screenshot (230)](https://user-images.githubusercontent.com/119657657/227710110-60b45428-b539-4b54-bd2e-6dc58ef8ff10.png)

![Screenshot (231)](https://user-images.githubusercontent.com/119657657/227710123-3578528f-bfe4-4d5b-b4f5-b5565ed9e8e5.png)

![Screenshot (232)](https://user-images.githubusercontent.com/119657657/227710137-a2fd02f6-5d7b-44cd-8c9f-3ba1c22bb9f6.png)

![Screenshot (233)](https://user-images.githubusercontent.com/119657657/227710146-642b1ced-a25e-4919-824d-1686fffe71a7.png)
