# 20210723_Reiff_Metis_EDA_Project
_This repo contains project scoping, MVP concepts, and accompanying analytical documentation/findings for the Metis EDA Module commenced Jul 2021_

---
### **Project scope**
* **Background:** Proprietary consumer research conducted by one of America's largest wireless telecom operators (ABC Telecom, 'ABC') suggests that a majority of New York commuters are unsatisfied with (free or limited free) public Wi-Fi bandwidth in Manhattan, and would be willing to supplement their cellular data plans with a paid subscription for fixed-access public Wi-Fi for $5-10/month. To address the most severely underserved neighborhoods in Manhattan, ABC is considering analyzing commuter traffic in tandem with current Wi-Fi hotspot density to identify areas of lowest bandwidth/commuter, under the assumption that highest bandwidth demand is during morning/evening commutes and lunch time. Assuming a successful commercial launch to underserved areas within Manhattan with a 3-month trial period beginning this July, ABC thinks its service can be more widely deployed throughout New York to meaningfully drive company earnings.    
* **Data & implementation:** The primary data sets leveraged for this analysis are **1)** NYC MTA turnstyle data as made available by the Metropolitan Transportation Authority (MTA) via free CSV files on the MTA website; and **2)** NYC public Wi-Fi hotspot locations provided by NYC OpenData for free via CSV. To gain a reasonable understanding of 'normalized' commuter traffic patterns in NYC pre- and post-COVID, I analyzed 9 months of turnstyle data (Apr-Jul 2021, Jul-Sept 2019, Jul-Sept 2018), though only the most recent cross-sectional data set for Wi-Fi hotspots was required.<br/><br/>

###### **Sample MTA data**
![sample_mta_data](https://github.com/reiffs/202107_Reiff_Metis_EDA_Project/blob/main/graphics/sample_mta_data.png)<br/><br/>
###### **NYC hotspots geographic**
![nyc_hotspots_geographic](https://github.com/reiffs/202107_Reiff_Metis_EDA_Project/blob/main/graphics/nyc_hotspots_geographic.png)<br/><br/>
###### **Sample NYC hotspot data (select data fields)**
![sample_nyc_hotspot_data](https://github.com/reiffs/202107_Reiff_Metis_EDA_Project/blob/main/graphics/sample_nyc_hotspot_data.png)<br/><br/>

* **Tool/technology requirements:** The MTA turnstyle data, hotspot data, and zip code maps to station (CSVs) was first ingested into a SQL database. I then joined the three data tables using SQLAlchemy to export to my Python environment for exploratory data analysis using Pandas. Visualizations were created predominantly with Matplotlib.pyplot, with supplemental tables/figures created in Microsoft Excel.     
* **Objective(s):** The minimum viable product resulting from this analysis seeks to identify areas of low Wi-Fi hotspot density relative to heavy commuter traffic as an actionable starting point for field testing ABC subscription hotspots throughout NYC.   

---
### **Findings/conclusions**
18 zip codes were identified based on criteria screening for low hotspot density (data points below the median density) while retaining reasonable commuter traffic (>75th percentile of commuter traffic). A cursory sensitivity analysis suggests this to be a multi-million dollar opportunity assuming modest adoption, using the price point in the background. 
