# 202107_Reiff_Metis_EDA_Project
_This repo contains project scoping, MVP concepts, and accompanying analytical documentation/findings for the Metis EDA Module commenced Jul 2021_

---
### **Project Scope**
* **Background:** Proprietary consumer research conducted by one of America's largest wireless telecom operators (ABC Telecom, 'ABC') suggests that a majority of New York commuters are unsatisfied with (free or limited free) public Wi-Fi bandwidth in Manhattan, and would be willing to supplement their cellular data plans with a paid subscription for fixed-access public Wi-Fi for up to $5/month. To address the most severely underserved neighborhoods in Manhattan, ABC is considering analyzing commuter traffic in tandem with current Wi-Fi hotspot density to identify areas of lowest bandwidth/commuter, under the assumption that highest bandwidth demand is during morning/evening commutes and lunch time. Assuming a successful commercial launch to underserved areas within Manhattan, ABC thinks its service can be more widely deloyed throughout New York to meaningfully drive company earnings.    
* **Data & Implementation:** The primary data sets leveraged for this analysis will be **1)** NYC MTA turnstyle data as made available by New York's Metro Transportation Authority (MTA) via free CSV files on the MTA website; and **2)** NYC public Wi-Fi hotspot locations provided by NYC OpenData for free via CSV. To gain a reasonable understanding of 'normalized' commuter traffic patterns in NYC pre- and post-COVID, this project will require at least 9 months of turnstyle data (Apr-Jul 2021, Apr-Jul 2020, Apr-Jul 2019), though only the most recent cross-sectional data set for Wi-Fi hotspots will be required.<br/><br/>

###### **Sample MTA Data**
![sample_mta_data](https://github.com/reiffs/202107_Reiff_Metis_EDA_Project/blob/main/sample_mta_data.png)<br/><br/>
###### **NYC Hotspots Geographic**
![nyc_hotspots_geographic](https://github.com/reiffs/202107_Reiff_Metis_EDA_Project/blob/main/nyc_hotspots_geographic.png)<br/><br/>
###### **Sample NYC Hotspot Data (Select Data Fields)**
![sample_nyc_hotspot_data](https://github.com/reiffs/202107_Reiff_Metis_EDA_Project/blob/main/sample_nyc_hotspot_data.png)<br/><br/>

* **Tool/Technology Requirements:** This project will require ingestion of the MTA turnstyle data (in the form of numerous CSVs) into a relational database table facilitated by Python; the NYC OpenData Wi-Fi data set is available in CSV format, and will be imported into a database table leveraging SQLite. The two data tables will be joined and refined in SQL before exporting to Python for exploratory data analysis leveraging Pandas and visualization utilizing Matplotlib and/or Seaborn (MS Excel may be used for non-computational visualization).     
* **Objective(s):** A minimum viable product resulting from this analysis will seek to identify areas of low Wi-Fi hotspot density relative to heavy commuter traffic. This analysis will be actionable as a starting point for field testing ABC subscription hotspots throughout Manhattan.   

---
### **Findings/Conclusions**
abcdefghijklmnopqrstuvwxyz
