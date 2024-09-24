This repository contains my final project for CSCA 5622: Introduction to Machine Learning: Supervised Learning at the University of Colorado, Boulder.

I wanted to find out how the Covid pandemic might have influenced the 2020 U.S. presidential election results. Although I can't prove causation given that there are so many factors that influence voting patterns, I hoped to use linear and logistic regression models to explore the question. My goals were: 

- Use logistic regression to predict, given a county's Covid death rate as of Nov. 3, 202, whether that county went to Biden or Trump in the 2020 election.
- Use linear regression on Covid death rate against counties' change in vote share between 2016 and 2020. In this analysis, only change in Republican/Democratic vote share (i.e. whether a county got redder or bluer, regardless of who actually won) was considered. A value of 0 means the vote share did not change in that county. A negative value means Biden got a higher share of votes in 2020 than Clinton did in 2016. A positive value means Trump got a higher share of votes in 2020 than he did in 2016. That means that even in a county Trump won in both years, the value could be negative if he won by a smaller margin in 2020.
  
I used the following data sources:
- Covid deaths by county as of Nov. 3, 2020: The New York Times. (2021). Coronavirus (Covid-19) Data in the United States. Retrieved Sept. 13, 2024, from https://github.com/nytimes/covid-19-data. (Full disclosure: I work at The New York Times.)
- Population estimates by county in 2020 (to calculate per-capita Covid death rates): United States Census Bureau. County Population Totals and Components of Change: 2020-2023. Retrieved Sept. 13, 2024 from https://www.census.gov/data/tables/time-series/demo/popest/2020s-counties-total.html.
- Vote totals in 2016 and 2020: MIT Election Data and Science Lab, 2018, "County Presidential Election Returns 2000-2020", https://doi.org/10.7910/DVN/VOQCHQ, Harvard Dataverse, V13, UNF:6:GILlTHRWH0LbH2TItBsb2w== [fileUNF].
