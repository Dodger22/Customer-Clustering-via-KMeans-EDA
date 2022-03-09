# Customer-Clustering-via-KMeans-EDA
I segmented a company's customers with KMeans clustering algorithm and made a customer personality analysis. I also performed exploratory data analysis on the data.
- The Plotly Library do not seems as output. You can reach the all of the visualization [https://www.kaggle.com/mirzazer/customer-clustering-via-kmeans-eda]

![Resim1](https://user-images.githubusercontent.com/88277713/157421000-392453c3-e3c9-4579-93a2-6c767b5a0235.png)

# Introduction
Customer Personality Analysis is a detailed analysis of a company’s ideal customers. It helps a business to better understand its customers and makes it easier for them to modify products according to the specific needs, behaviors and concerns of different types of customers. Customer personality analysis helps a business to modify its product based on its target customers from different types of customer segments. For example, instead of spending money to market a new product to every customer in the company’s database, a company can analyze which customer segment is most likely to buy the product and then market the product only on that particular segment.
I got the Customer Informatıon Dataset from Kaggle. I will try to analyze customer personalities by applying a clustering algorithm to the company's customer information and ensure that the company applies special campaigns, opportunuties and discount coupons accordingly.

![Resim2](https://user-images.githubusercontent.com/88277713/157421153-08edb8eb-b0d3-44c9-8ebe-d2e5d8861abf.png)

The dataset has 29 features and 2240 entries.I carried out the work with the Python programming language. I first examined the dataset, then corrected the types of features, filled in missing data by averaging other data by type, found no noisy data, and deleted outliers.

I used Boxplot, Distplot, Correlation , and Bar charts while implementing Exploratory Data Analysis. I have standardized the data for PCA. After all this process, I applied PCA (Principal Component Analysis) to the data and reduced the data size (0.95 variance). So I can apply faster. Then I figured out how many cluster entries I need to make for the KMeans clustering algorithm using the Elbow Method. I applied it to the KMeans clustering algorithm and as you can see on the left, 3 different clusters were formed. I divided these clusters into SEGMENT I, II and III.

![Resim3](https://user-images.githubusercontent.com/88277713/157421323-3f03bcf0-e25f-4131-8f0a-4026a9578bfe.png)

I examined the 3 Segments we created by making visualizations. With bagel charts, I discovered which products the clusters you see on the left spend more on. In general, I see the customers' inclination towards Wine, but Segment II is far ahead in this sense. Then comes the meat, the golden fish. In the correlation analysis, I saw that those who buy wine definitely also buy meat.

![Resim4](https://user-images.githubusercontent.com/88277713/157421427-14606d0f-b13a-4c65-8e6c-077f07906c3b.png)

I visualized in which areas the segments were shopping with barplot, then I examined the monthly website visit rate and the complaint rates for 2 years.I saw that the complaint rates were higher in Segment I and I discovered that Segment I  also did less catalog shopping.

By examining customer revenues with Distplot, I saw that Segment III had more revenue, followed by segment II and segment I. I noticed that the distribution ratios were similar in all three segments.

![Resim5](https://user-images.githubusercontent.com/88277713/157421507-0cd8e904-5453-4267-a8f3-8c4479f9a880.png)


![Resim6](https://user-images.githubusercontent.com/88277713/157421570-7a4754f1-2a1a-49a7-83f2-cf66b72f8583.png)

I set age ranges for customers and visualized Segments by age ranges. In general, there is a large number of customers between the ages of 36-60 in all segments. There are almost no people aged 19-35 in segment II. The number of people over the age of 61 who shop from the company is quite high. A maximum age of 89 might count as an outlier, but I didn't fix it. Because I thought that an 89-year old person could also shop. It is also very interesting that the company has no customers under the age of 18.

The table below shows the number of children in the household according to the marriage status of the customers according to the clusters.

![Resim7](https://user-images.githubusercontent.com/88277713/157421648-f2334e5f-0252-4ed9-bf58-b5acf30efd35.png)



