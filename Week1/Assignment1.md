***In the notes of Week 1, we compared & contrasted MLOps with DevOps. In this question, you need to understand what is meant by the term AIOps, & then contrast it with MLOps.***

AIOps is the application of artificial intelligence to IT operations. Modern IT environments generate immense quantities of highly complex data that needs to be monitored and managed.  With the help of AI and ML algorithms, IT Ops and DevOps teams in organisations can identify issues earlier and resolve them quickly without the business being affected.  AIOps provides IT operations a real-time understanding of issues that can affect the availability and performance of Digital services.

Organisations generally deploy AIOps as an independent platform that ingests information from all IT monitoring devices and acts as a central system of engagement. This platform has five key algorithms that help in automating and streamlining the main IT operations monitoring processes - *data selection, pattern discovery, inference, collaboration,* and *automation.*

![AIOps algos](/Images/AIOps.jpg)

It removes noise and duplication in the ingested data. After grouping and correlating the revelant data, it discovers patterns, draws inference and communicates the results of the analysis to the Ops team who can then quickly resolve any issues. The AIOps platform stores the causes and solutions for every fixed incident, and uses that knowledge to help Ops teams diagnose causes and prescribe solutions for future issues.

While AIOps augments the IT Ops, MLOps is a set of practices that are followed to ensure that ML is reproducible, collaborative, scalable and continuous. MLOps focuses on specific aspects of machine learning lifecycle management - *data preparation, model training and tuning, deployment* and *monitoring.* Meanwhile AIOps enhances the general IT operations by optimizing the problem-resolution workflow so that it can be performed faster, more precisely, and with fewer manual processes.

<hr>

***Interpretable Machine Learning is another concept that has attracted lot of attention recently & is promoted by most of the MLOps frameworks. Explain what it means for a linear regression model to be interpretable.***

A machine learning model is said to be interpretable if we can graphically visualize and intuitively understand the outputs of the model and their implications. Out of all machine learning models linear regression is the simplest one, making it the easiest to understand intuitively. A linear regression model outputs the weights corresponding to each feature of the model which can be understood intuitively as explained below. 

The interpretation of a weight depends on the type that feature. If the feature is numerical it means that increasing the numerical feature by one unit changes the estimated outcome by its weight. Similarly, for a categorical feature changing the choice of category from one to another would change the output correspondingly. The intercept or the weight of the constant feature can be interpreted as the outcome when all features are standardised and at their mean value. 

Other methods used to interpret the linear regression model are the R-squared measurement and t-statistic. R-squared depicts how much of the total variance of the target outcome is explained by the model. The higher R-squared, the better the model explains the data and the more meaningful the weights are. To measure the importance of a particular feature, the absolute value of the t-statistic can be used.

Furthermore, a weight plot and an effect plot can be used to visually understand our model's outputs. A weight plot shows the weights and their standard deviation for every feature. Standardising the data before fitting the linear model would make the weight plot more practical. As all the features will be on a similar scale, comparison of their weights would be more significant. An effect plot too makes it easy to understand the relationship between the features and the outcome.

<hr>

***AWS Free Tier account***

![AWS account](/Images/AWS.png)

<hr>

***References***

A detailed guide to [AIOps](https://www.moogsoft.com/resources/aiops/guide/everything-aiops/#seven) and [interpretable ML](https://christophm.github.io/interpretable-ml-book/limo.html)!
