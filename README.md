# 20210723_Reiff_Metis_EDA_Project
_This repo contains project scoping, MVP concepts, and accompanying analytical documentation/findings for the Metis EDA Module commenced Jul 2021_

---
### **Project scope**
* **Background:** Proprietary consumer research conducted by one of America's largest wireless telecom operators (ABC Telecom, 'ABC') suggests that a majority of New York commuters are unsatisfied with (free or limited free) public Wi-Fi bandwidth in Manhattan, and would be willing to supplement their cellular data plans with a paid subscription for fixed-access public Wi-Fi for $5-10/month. To address the most severely underserved neighborhoods in Manhattan, ABC is considering analyzing commuter traffic in tandem with current Wi-Fi hotspot density to identify areas of lowest bandwidth/commuter, under the assumption that highest bandwidth demand is during morning/evening commutes and lunch time. Assuming a successful commercial launch to underserved areas within Manhattan with a 3-month trial period beginning this July, ABC thinks its service can be more widely deployed throughout New York to meaningfully drive company earnings.    
* **Data & implementation:** The primary data sets leveraged for this analysis will be **1)** NYC MTA turnstyle data as made available by the Metropolitan Transportation Authority (MTA) via free CSV files on the MTA website; and **2)** NYC public Wi-Fi hotspot locations provided by NYC OpenData for free via CSV. To gain a reasonable understanding of 'normalized' commuter traffic patterns in NYC pre- and post-COVID, this project will require at least 9 months of turnstyle data (Apr-Jul 2021, Jul-Sept 2019, Jul-Sept 2018), though only the most recent cross-sectional data set for Wi-Fi hotspots will be required.<br/><br/>

###### **Sample MTA data**
![sample_mta_data](https://github.com/reiffs/202107_Reiff_Metis_EDA_Project/blob/main/graphics/sample_mta_data.png)<br/><br/>
###### **NYC hotspots geographic**
![nyc_hotspots_geographic](https://github.com/reiffs/202107_Reiff_Metis_EDA_Project/blob/main/graphics/nyc_hotspots_geographic.png)<br/><br/>
###### **Sample NYC hotspot data (select data fields)**
![sample_nyc_hotspot_data](https://github.com/reiffs/202107_Reiff_Metis_EDA_Project/blob/main/graphics/sample_nyc_hotspot_data.png)<br/><br/>

* **Tool/technology requirements:** This project will require ingestion of the MTA turnstyle data (in the form of numerous CSVs) into a relational database table facilitated by Python; the NYC OpenData Wi-Fi data set is available in CSV format, and will be imported into a database table leveraging SQLite. The two data tables will be joined and refined in SQL before exporting to Python for exploratory data analysis leveraging Pandas and visualization utilizing Matplotlib and/or Seaborn (MS Excel may be used for non-computational visualization).     
* **Objective(s):** A minimum viable product resulting from this analysis will seek to identify areas of low Wi-Fi hotspot density relative to heavy commuter traffic. This analysis will be actionable as a starting point for field testing ABC subscription hotspots throughout Manhattan.   

---
### **Findings/conclusions**
abcdefghijklmnopqrstuvwxyz
