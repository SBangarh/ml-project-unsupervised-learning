# machine_learning_project-unsupervised-learning

## Goals
1. Continue to apply python best practices
2. Develop EDA techniques a bit more - explore other ways to handle outliers and nulls,
3. Work to increase efficiency using functions and data pipelines
4. Develop a unsupervised ML model to cluster my data
5. Have fun

## Process
First thing I did was import my libraries and develop functions for my EDA. These functions ranged from understanding the data to visualizing the data. I performed EDA using these functions and explored the data using a top down approach. I started at the dataframe level to understand the data and build visuals to communicate the data. I went to feature specific level after determining relationships and behaviours across the channels and regions.

I identified outliers using code and boxplots. I explored removing the outliers, median imputation, log transformation, and winsorization. I settled on winsorization as it, to a degree, allowed for extreme values and removed outliers, whereas the other methods still had outliers and the distribution changed.

Next, I explored clustering with Kmeans and heirarchial clustering. I didn't really explore doing any optimizing via GridsearchCV due to time contraints, but it is something I aim to explore.
I performed these these algorithms multiple times for comparison. My process was to initially guess, perform a optimization method, re-run an optimized cluster model, then, if necessary, manually tune the optimal number of clusters. 


## Results
1. Channel 1 (Hotels/Restaurants/Cafes) accounted for almost 2X more transactions than channel 2 (Retail); however, The difference in sales was approximately 1.5M; 
2. Other regions accounted for the most transactions and sales for both channels;
3. The Channels spent differently with respect to categories as well where Fresh dominated for Channel 1 and Grocery dominated for Channel 2; 
4. Kmeans was interesting as the Elbow Method indicated the optimal number of clusters would be 3, but this resulted in too close of a proximity for two clusters. Two clusters appeared to work better;
5. Heirarchial clustering was also weird. Output was unexpected, so hard to interpret there. Will have to revisit most likely;
6. PCA indicated, for the most part, two distinct classes that explained ~63% of the variance. 

## Challenges
1. Understanding the backend of the models I used. I need to invest more time in the theory behind the code.
2. Related to above, but I had trouble interpreting my model results.
3. Ambiguity, I'm getting more comfortable with it, but still can improve.
4. Establishing a workflow - things got murky when we started supervised learning

## Future goals
1. Improve my understanding of the theory behind the models and how it works
2. Apply models I have learned to data that is not project related
3. Explore model inputs and learn to bridge my data distribution to the optimal model
4. Play around with feature engineering a bit more; there is more information in the data
5. Write a bit more clean code, I used pipeline and functions, but the notebook tidyness can definitely improve.
6. Keep having fun