# General Description
The work sample is from the NYC City Bike dataset in Google BigQuery. You can access the data from this link: https://console.cloud.google.com/marketplace/details/city-of-new-york/nyc-citi-bike

I'm answering questions below: <br/>
(which include SQL code to draw data structure from the Google BigQuery, and Python code to impletment statistical analysis and visulize results.)
* Q1: What is the trip duration distribution of Citibike trips?
* Q2: What is the most popular Citibike trip? 
* Q3: Were there new bike stations introduced or removed at any point in time? What makes you think it were or weren't?

# Answer:
* Q1:<br/>
Lognormal distribution.<br/>
The parameter of the lognormal distribution is 0.7740207642832148, 20.943962974413324, and 614.3445916251605 <br/>
<img src="https://drive.google.com/uc?export=view&id=18ckLoHDt8jLHdY4x82Ski6O4U6MBIiU2"  width="500" height="350">

* Q2:<br/>
According to the data, the highest numbers of trip is from "Central Park S & 6 Ave" to "Central Park S & 6 Ave", which is 47215 times. **However**, it seems the highest four numbers of trip are **not** "trip" at all, since they rent and returned at the same stop. It might be the testing sets which was recorded in this data.<br/>
If we look at the highest number of trip which rent and returned at different station, it is from **"12 Ave & W 40 St"** to **"West St & Chambers St"**, which was recorded **12417 times** of renting. <br/>

* Q3:<br/>
Detail answer please view the code. Below shows the visualization of service dates of every stations.
<img src="https://drive.google.com/uc?export=view&id=1mRCi4cIM5_wuiW8f2ZJBel4Z4NYC5drO"  width="1000" height="400">
<img src="https://drive.google.com/uc?export=view&id=1JtOdmk0SDsIW5LxOdsYE4ELUeg8jPoNj"  width="1000" height="400">
<img src="https://drive.google.com/uc?export=view&id=1S0-weiZxzxMNSUkpcG2Wke1bbm1WGMw-"  width="1000" height="400">
<img src="https://drive.google.com/uc?export=view&id=1UyRBuwhItyk-jtCaFe7QSg_fmTFozB2k"  width="1000" height="650">
<img src="https://drive.google.com/uc?export=view&id=1GaFLi_mkGNbAMd5osZofOCg_5SY3ZTe1"  width="1000" height="650">
<img src="https://drive.google.com/uc?export=view&id=13fulQlW2qpi2Roh2eEMCsa-ITnz6EC-s"  width="1000" height="400">

* Appendix: Draw Geomap<br/>
Since I would also like to know exact locations of stations and its popularity, I also draw a Geomap to better understand the relationship.
<img src="https://drive.google.com/uc?export=view&id=1aat6eI8PwGBk3cbOm0DJS1z1PmChr5F0"  width="800" height="560">
