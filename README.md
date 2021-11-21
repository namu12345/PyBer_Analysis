# Overview 

# PyBer_Analysis :
The Pyber_Analysis is analysis of hypothetical ride-sharing app company "Pyber". In this project I'll be helping out Omar(manager of Pyber) to analyze all the rideshare data from January to early May of 2019 and create a compelling visualization for the CEO, V. Isualize.

# Purpose of Pyber_Analysis :
The purpose of our analysis is to create a summary dataframe that will show ride sharing data by city type(Rural,Urban & Suburban). Once we find our data we are going to create a multiple line graph that shows total weekly fares by each city type. How we first pulled our data is by using the pandas Groupby() function with the count() and sum () to get the total number of drivers,rides and fares by city type. Once we pulled this information and assigned it to functions we were able to calculate our average fare per ride and driver. Once we had all of that information together we were able to format into a newdata frame and re-format the columns. We further created the Pivot Table to get the total fares for each type of city by the date. And then finally we used our resample function to get the weekly sum of fares of each city. And our last section was to create visualization data in the form of line chart for CEO V.Isualize.

# Results :
As mentioned earlier we started our analysis by using the Pandas groupby() function with the count() and sum() methods on PyBer DataFrame columns to get the total number of rides, total number of drivers, and the total fares for each city type. Then we calculated the average fare per ride and average fare per driver for each city type. Finally, we added the data to a new DataFrame wherein we did formatted our columns to have better understanding. 

- The results are as below :

![image](https://user-images.githubusercontent.com/92283185/142744582-5507cf85-ce5f-4de0-b376-80d26a1bb19c.png)
![image](https://user-images.githubusercontent.com/92283185/142744590-8717de5c-a1c5-4d11-bbd0-abca41077c81.png)

- And after cleaning & formatting the dataframe it looks like :

![image](https://user-images.githubusercontent.com/92283185/142744619-983fc56a-02b2-4457-b73e-410aeed88a8d.png)

Further in analysis we used our Pandas skills and also used two new functions, pivot() and resample() to create a multiple-line graph that showed the total fares for each week by city type. To work on Pivot and resampling we started with grouping our data by using groupby function on the "type" and "date" columns of the pyber_data_df DataFrame, then applied the sum() method on the "fare" column to show the total fare amount for each date. 

- This resulted in the following way :

![image](https://user-images.githubusercontent.com/92283185/142744747-fedb45e4-e86a-40cd-a5f1-11bc06f6338b.png)

- Now we had to reset our index on the DataFrame which we created right in starting. This is needed to use the 'pivot()' function later in our analysis. This is how i reset my index :

![image](https://user-images.githubusercontent.com/92283185/142744772-055bb389-95af-4dba-a394-d6d9d878d0eb.png)

- After reseting the index we created the Pivot table by using pivot function which resulted as below : 

![image](https://user-images.githubusercontent.com/92283185/142744814-ef93c03d-a906-4def-8373-2664161710a3.png)

- Since we are looking for the data from January to early May 2019 we created new pivot table by using the loc method on the date range from 2019-01-01 through 2019-04-28.
And it resulted in below image :

![image](https://user-images.githubusercontent.com/92283185/142744933-c2c877c8-5496-4a6f-8d22-96e22b0875e0.png)

- Our final step is to Resample the data in weekly bins to get the total fares for each week. For resampling, first we have to set the "date" index to datetime datatype. So  following is the results of both changing the datatype of date column and resample the data to see total fares for each week:

![image](https://user-images.githubusercontent.com/92283185/142745113-81a0f3dd-30f1-410b-886d-a2d1d07463b8.png)

- Resample :

![image](https://user-images.githubusercontent.com/92283185/142745138-0394c93a-55a0-4ed7-995c-04cf1a322067.png)

The last section of our analysis is to visualize our data in graphical way. This is done by 








