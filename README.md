# Bank Customer Segmentation

## The Situation
You've just been hired as a Data Scientist for the Bank of Mavenland, the national bank in the country where data analysis is the most popular pastime.

## The Assignment
The product team at the Bank of Mavenland wants to find ways to better cater to their different segments of customers.
You've been asked to segment their current customers and recommend potential new products or services for each segment.

## The Objectives
1. Prepare the data
2. Cluster the customers (round 1)
3. Cluster the customers (round 2)
4. Explore the clusters and make recommendations

## The Data Set

#### Bank Customer Churn
Account information for 10,000 customers at a European bank, including details on their credit score, balance, products, and whether they have churned.

(the Bank_Churn_Messy.xslx file is included for completing the Bank Customer Data Prep)

#### Recommended Analysis
1. What attributes are more common among churners than non-churners? Can churn be predicted using the variables in the data?
2. What do the overall demographics of the bank's customers look like?
3. Is there a difference between German, French, and Spanish customers in terms of account behavior?
4. What types of segments exist within the bank's customers?

#### Objective 1: Prepare the data for modeling
Your first objective is to prepare the data for modeling by selecting a subset of fields, making sure they are numeric, looking at their distributions, and engineering a new feature.

* Read the "Bank_Churn.csv" file and preview the top 5 rows.
* Create a DataFrame containing all fields except "CustomerId", "Surname" and "Exited".
* Make all text fields numeric.
* Explore the data by looking at the min/max values and the distribution of each column.
* Engineer a new feature called "ProductsPerYear".

#### Objective 2: Cluster the customers (round 1)
Your second objective is to segment the customers using K-Means clustering, including standardizing the data, creating an inertia plot, and interpreting the clusters.

* Standardize the data so that each column has a mean of 0 and standard deviation of 1.
* Fit K-Means Clustering models on the standardized data with 2-15 clusters to create an inertia plot.
* Identify the elbow of the inertia plot and fit a K-Means model using that value of k.
* Check the number of customers in each cluster.
* Create a heat map of cluster centers and interpret the clusters.

#### Objective 3: Cluster the customers (round 2)
Your third objective is to segment the customers using K-Means clustering using a different subset of fields and compare the model results.

* Take a look at the summary stats by country and exclude the country fields.
* Fit K-Means Clustering models on the standardized data without country fields with 2-15 clusters to create an inertia plot.
* Identify the elbow of the inertia plot and fit a K-Means model using that value of k.
* Check the number of customers in each cluster.
* Create a heat map of cluster centers and interpret the clusters.

#### Objective 4: Explore the clusters and make recommendations
Your final objective is to further explore your K-Means clusters by looking at their churn rate and country breakdown, then make recommendations for how to cater to each one.

* Create a DataFrame that combines the data set from the end of Objective 1, the "Exited" field, and the cluster labels.
* View the churn rate (% of customers who "Exited") for each cluster.
* View the country breakdown for each cluster.
* Make recommendations for how to cater to each customer segment.

#### [Project Link]()