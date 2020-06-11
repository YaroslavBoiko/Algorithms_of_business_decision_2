So, in this practical work up to week two 2, I: 

	1. I used HBSCAN and c-means clustering methods for the data I used in the previous work:   https://github.com/YaroslavBoiko/Algorithms_of_business_decision
  Job description: To implement these methods: I used the existing libraries: hdbscan (for HDBSCAN implementation) and FCM (for c-means application).

	
| Algorithm     | Silhouette Score | Davies-Bouldin score |
| :------------ |:----------------:| -----:|
| DBSCAN        | 0.44		        | 0.43  |
| KMeans        | 0.32             | 1.09  |
| HBSCAN 	      | 0.12             | 1.67  |
| CMeans      	| 0.17             | 1.32  |

When viewing the results of new algorithms that I used, in general, new algorithms are less clustered than previous ones. If we analyze whether HBSCAN or CMeans is better, then unexpectedly CMeans is better to show the estimates in the table.

Description of results and analysis of results:
To evaluate the results of clustering, as in the previous work, I used Silhouette Score and Davies-Bouldin score. You can see the results of the clustering algorithms below.



	2. Took and used Survival data and applied KM and Cox estimators on these data; Made some conclusions.

So in this task, data that I took is the duration of the person in the office.

After the data was successfully downloaded, I used the existing lifeness library to implement the Kaplan-Meier estimator on the data I downloaded.
The results of the model I made can be seen in the plot below. As you can see, this plot shows the probability that a person will be in a managerial position for a certain number of years (y-axis - probability, x - number of years in office)

<img src="https://github.com/YaroslavBoiko/Algorithms_of_business_decision_2/blob/master/plots/4.png" width="250" height="250">


After successfully testing the Kaplan-Meier estimator, I tested the COX estimator, for which I also chose the lifeness library. But the data, I chose others -data on the crime in a particular week. A number of visualizations were also performed to understand the results.

<img src="https://github.com/YaroslavBoiko/Algorithms_of_business_decision_2/blob/master/plots/2.png" width="250" height="250">, <img src="https://github.com/YaroslavBoiko/Algorithms_of_business_decision_2/blob/master/plots/3.png" width="250" height="250">

I was also interested to see the difference between KM estimator and Cox estimators, so I used KM estimation for the second dataset (survival date, which I used for COX estimation).
In conclusion, Cox estimator is more optimistic in its forecasts (which is reflected in the assessment of the probability of incidents per week)

<img src="https://github.com/YaroslavBoiko/Algorithms_of_business_decision_2/blob/master/plots/1.png" width="250" height="250">, <img src="https://github.com/YaroslavBoiko/Algorithms_of_business_decision_2/blob/master/plots/2.png" width="250" height="250">
