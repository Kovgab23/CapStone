# CapStone Project for IBM data science program

## Repository of exam files

Above files are here as proof of accomplishment.

Problem statement:
we are to predict if the Falcon 9 first stage will land successfully. SpaceX advertises Falcon 9 rocket launches on its website, with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings is because SpaceX can reuse the first stage. Therefore if we can determine if the first stage will land, we can determine the cost of a launch. This information can be used if an alternate company wants to bid against SpaceX for a rocket launch. ​

Objective:

Determine the best conditions of rocket launch to recognize characteristics promote successful landing​

What are the attributes most important to focus on to improve successful landing rate?​

Methodologies:
Data collection methodology:​

Obtained by both Json Apis and Webscraping of Wikipages with Beautifulsoap package to webscrape HTML tables​

Perform data wrangling​

Wrangling data using an Api, sampling data and dealing with null values​

Perform exploratory data analysis (EDA) using visualization and SQL​

Perform interactive visual analytics using Folium and Plotly Dash​

Perform predictive analysis using classification models​

Results:
Exploratory data analysis results​

There are 4 launch sites used by SpaceX​

Total Payload Mass (Kg) carried launched by Nasa is 45,596​

The average payload mass (kg) carried by Booster version F9 v1.1 is 2,535 kg​

The 1st successful landing by a drone ship was at 04/08/2016​

We can specifically list the booster version in a given payload mass range which landed on a ground pad​

We applied the aggregate function to see nr of total success vs total failures: 61 vs 40​

And we restrict results just for a given year to see the subtotal of landing outcomes​

Predictive analysis results​

Logistic regression, SVM and K-nearest neighbors, all of these three methods give the best performance, with accuracy of 0.83​

Parameters need to be fine tuned for rockets launched for different purposes (depending on payload mass or target orbit for instance)​

The most secure landing outcome can be characterized by the following attributes:​

Initial launch: KSC LC-39A, Payload Mass in range of: below 6000 or above 8000, Booster version: FT or B4​

Regarding target orbit:​

For the lower range of payload mass SSO possess and outstanding success rate​

While on the high payload mass range more data needed to stress the statement that orbits ISS or PO are secure ​

Although there are 3 model shows similarly good fit for our problem constant evaluation and test is need going forward as more and more data is available​
