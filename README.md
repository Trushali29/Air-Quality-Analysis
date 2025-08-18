# Conduct Product Market Fit Research for Air Purifier Development Using AQI Analytics

This is the Resume Project for conducting a product market fit analysis on air purifiers. This challenge is powered by Codebasics platform and sponsored by dataful platform for providing data to gain insights.

## **PROBLEM STATEMENT** 

According to the IQ air reports around the world there are 20 air polluted urban cities which have higher AQI index out of which 14 cities are from India.

To Tackle with this AirPure Innovations is a startup born out of the air quality crisis in India. The company is in the early stages of the product development and is unsure whether there is a strong, sustained demand for its air purifier product.

 They want to understand the patterns of the AQI across Indian states before committing to Production and R\&D by answering the critical questions: 

1. What pollutants or particles should their air purifier target?  
2. What are the most essential features that should be incorporated into the air purifier?  
3. Which cities have the highest demand for air purifiers, and what is the market size in these regions?  
4. How can R\&D be aligned with localized pollution patterns?

## **Dataset Information**

**Dataset: Day-wise, State-wise Air Quality Index (AQI) of Major Cities and Towns in India**

This dataset contains daily Air Quality Index (AQI) values for various cities and towns across different states in India. It records air quality trends to help analyze pollution levels over time and across regions.

**Geographical Scope**  
India (State-wise and City/Town-wise)

**Time Coverage:**  
Daily observations (Specify actual date range if known, e.g., Jan 2022– May 2025\)

**Columns Description:** 

| Column Name | Data Type | Description |
| ----- | ----- | ----- |
| Date | Date (dd-mm-yyyy) | The specific day on which the AQI measurement was recorded |
| State | Text | The name of the Indian state where the city/town is located |
| City | Text | The name of the city or town where the AQI was measured |
| AQI | Numeric | The Air Quality Index value indicating the level of air pollution for that day |

**Dataset: State, District, and Disease-wise Cases and Deaths reported due to Outbreak of Diseases as per Weekly reports under IDSP**

This dataset records weekly outbreak data of various diseases across Indian states and districts, as collected under the Integrated Disease Surveillance Programme (IDSP). It includes the number of reported cases and deaths for specific diseases during each epidemiological week. This data helps monitor and respond to public health threats.

**Geographical Scope:** India – State-wise and District-wise coverage

**Time Coverage:** Weekly reports ( from year 2022 to 2025, week 1 to 52\)

| Column Name | Data Type | Description |
| ----- | ----- | ----- |
| State | Text | Name of the Indian state where the disease outbreak occurred |
| District | Text | Name of the district within the state where the disease was reported |
| Year | Numeric | The calendar year when the outbreak was reported |
| Week | Numeric | Epidemiological week number (1–52) in which the data was recorded |
| Disease Name | Text | Name of the specific disease reported during the week |
| No. of Cases | Numeric | Total number of reported or confirmed disease cases in that week and district |
| No. of Deaths | Numeric | Total number of deaths reported due to the disease in the same week and district |
| Status  | Text  | Whether the Illness was Reported, Reported Late, Reported in Same Week or Previous Week Follow up  |

**Dataset: State, Vehicle Class and Fuel Type-wise Total Number of Vehicles Registered in Each Month in India**

This dataset contains monthly records of the number of vehicles registered in India, categorized by state, vehicle class (e.g., two-wheeler, car, bus), and fuel type (e.g., petrol, diesel, electric). It provides insights into vehicle registration trends across different states and fuel categories over time.

**Time Coverage:** Monthly coverage from year 2022 till 2025

| Column Name | Data Type | Description |
| ----- | ----- | ----- |
| State | Text | Name of the Indian state where the vehicles were registered |
| Month | Text / Date | Month and year of vehicle registration (e.g., Jan-2023) |
| Vehicle Class | Text | Category/type of vehicle (e.g., Two-Wheeler, LMV, HMV, Bus, etc.) |
| Fuel Type | Text | Type of fuel the vehicle uses (e.g., Petrol, Diesel, Electric, CNG) |
| Number of Vehicles | Numeric | Total number of vehicles registered under the given category in that month |

**Dataset: Population Projection of India: State- and Gender-wise Yearly Projected Urban Population (2011-2036)**

This dataset provides projected urban population figures for Indian states, disaggregated by gender (male and female) for each year from 2011 to 2036\. These projections are based on estimates from official census data and demographic models, and are intended for use in urban planning, resource allocation, and policy formulation.

**Time Coverage:** From year 2011 \- 2036 monthly data.

| Column Name | Data Type | Description |
| ----- | ----- | ----- |
| State | Text | Name of the Indian state |
| Year | Numeric | Year of the projected population (ranging from 2011 to 2036\) |
| Male Population | Numeric | Projected urban male population for the specified state and year |
| Female Population | Numeric | Projected urban female population for the specified state and year |
| Total Population | Numeric | Sum of projected male and female urban population for that state and year |

## **PRIMARY QUESTIONS**

### **List the top 5 and bottom 5 areas with highest average AQI. (Consider areas which contains data from last 6 months: December 2024 to May 2025\)**

**Bottom 5 areas**

- It shows areas with lowest AQI that can be 33.31 which if of state Tirunelveli 

In the top 5 areas it shows Byrnihat (Meghalaya) with 284.19 aqi, Delhi as the second position with 238.92.   
The reason for **Bynihat to be on top is due to its industrialization environment.** There are many industries of machinery, distillery, cement and steel. Also its geographical environment location on the Assam-Meghalaya border, with its unique topography, consists of a low pressure zone which traps pollutants and makes it unable to disperse.

**Reasons for high AQI** 

- Seasonal stubble Burning in agricultural areas   
- Industrial activity  
- Geographical location factor low air pressure which can trap pollutants in air  
- Constructions and vehicular emission

The AQI in Chamarajanagar, Vijayapura, Madikeri (Karnataka), and Tirunelveli (Tamil Nadu), including the border area of Palkalaiperur, is likely low due to a combination of factors such as **lower industrial activity, less population density, and potentially more green cover**. These areas are not major industrial hubs and have a relatively smaller population compared to larger cities, which contributes to better air quality.

### **List out top 2 and bottom 2 prominent pollutants for each state of southern India.  (Consider data post covid: 2022 onwards)**

PM10 and PM2.5 stand out as the top pollutants across southern states while few other pollutants such NH3, NO2, O3, and SO2. The factors could be more vehicles and construction and demolition duct and debris. 

### **Does AQI improve on weekends vs weekdays in Indian metro cities (Delhi, Mumbai, Chennai, Kolkata, Bengaluru, Hyderabad, Ahmedabad, Pune)?(Consider data from last 1 year)**

There is a slight improvement in AQI for each metro city with no huge difference between AQI on weekdays and weekends. 

**Monthly chart of each states**   
It shows months from April to mid \- October and seasonal time for monsoon where AQI has a sudden drop which is normal for every state.

During the month of Oct \- Jan the AQI is at its peak the factors could be harvesting seasonal in which stubble burning is done around those states. 

### **Which months consistently show the worst air quality across Indian states (Consider top 10 states with high distinct areas)**

Months of January, February and December show signs of high AQI. While November is a leading month in most all those states. 

Months ranging from Mid-April or May till September we can see there is a sudden drop of the AQI for this a dominant factor can be a monsoon season. 

After the monsoon season, harvesting seasons start for various states in different timelines so we can see there is a rise of AQI level from October till Jan and more or less it can expand till April. Depends on the state's geographical location.

As we see in the line chart there is only a slight difference between weekday and weekend AQI levels.

### **For the city of Bengaluru, how many days fell under each air quality category (e.g., Good, Moderate, Poor, etc.) between March and May 2025?**

In the Pie chart we see that Bengaluru has 13 days with moderate level AQI and 48 days with Satisfactory level AQI. 

### **List the top two most reported disease illnesses in each state over the past three years, along with the corresponding average Air Quality Index (AQI) for that period.**

Based on the reports of the table we can see two most prominent diseases are Acute Diarrheal Disease and Food Poisoning. 

Kerala, Maharashtra, Karnataka, Odisha, Chhattisgarh tops the chart with more disease cases. In terms of AQI Delhi, Jharkhand, Himachal Pradesh, Bihar, Chandigarh tops the list having highest AQI in the past 3 years but their disease cases are not that correlated with the AQI levels.

### **List the top 5 states with high EV adoption and analyse if their average AQI is significantly better compared to states with lower EV adoption.**

The EV fuels selected are Electric (BOV), Fuel Cell Hydrogen, Plug-in Hybrid EV, Pure EV, Solar and Strong Hybrid EV. 

Uttar Pradesh, Maharashtra, Karnataka, Tamil Nadu and Rajasthan rank as the top 5 states with High EVs registration. Their overall average AQI is 101.27 which is pretty less than the overall average AQI of other states which is 119.53. It can be the reason that EVs have played a better role in reducing AQI levels. 

## **SECONDARY QUESTION** 

### **Which age group is most affected by air pollution-related health outcomes and how does this vary by city?**

**Source 1:  Air Pollution and Mortality in India: Investigating the Nexus of Ambient and Household Pollution Across Life Stages ( Research paper )**

This report examines the **adverse health effects of PM2.5 pollutants originating from household kitchens in India**. Analysis indicates that in urban areas, every 10-unit rise in PM10 levels is associated with a **6% increase in neonatal mortality and an 8% rise in premature deaths.**

Geographical Distribution of PM2.5 Concentrations  
**High levels:** The Indo-Gangetic Plain, including the National Capital Region (NCR) and parts of southern West Bengal.  
**Low levels:** Northern high-elevation states such as Arunachal Pradesh, Sikkim, Uttarakhand, Himachal Pradesh, Jammu & Kashmir, and Ladakh, as well as Kerala, western Karnataka, and selected southern districts of Tamil Nadu.

**Source 2: Times of India Report  \- Air Pollution Impact on Young children in India**

Air pollution has been identified as the second most significant health risk factor in India, following hypertension. According to the State of Global Air (SoGA) 2024 ( by an US based organization Health Effects Institute ) in 2021, an estimated 2.1 million deaths in India were attributable to air pollution, out of a global total of 8.1 million.

**Health Impacts in 2021**

* **Cardiovascular diseases:** 40% of heart disease deaths are linked to air pollution.  
* **Respiratory diseases:** 33% of lung cancer deaths and 70% of chronic obstructive pulmonary disease (COPD) deaths associated with air pollution.  
* **Metabolic diseases:** 20% of type 2 diabetes deaths related to air pollution exposure.  
* **Neurological impacts:** 41% of stroke deaths connected to air pollution.

**Impact on Children**  
In 2021, over 700,000 deaths among children under five years of age were attributed to air pollution. Pneumonia and asthma were identified as the most prevalent illnesses affecting children in this age group.

### **Who are the major competitors in the Indian air purifier market, and what are their key differentiators (e.g., price, filtration stages, smart features)?**

**Eureka Forbes Smart Air Purifier 355**

* **Coverage Area:** 200–500 sq. ft. (Living rooms up to 480 sq. ft., Bedrooms)  
* **Category:** Quick Cleaning & Ionization  
* **Filtration Stages:** Pre-Filter \+ Activated Carbon Filter \+ True H13 HEPA Filter \+ Plasma Filter  
* **Smart Features:** WiFi Enabled, PM 2.5 value digital display, Activated Carbon Filter, Purifies air within 10 mins  
* **Price Range:** ₹500 – ₹20,000

**Philips Air Purifier 1000i Series (AC1715)**

* **Coverage Area:** 300–800 sq. ft. (Medium & Large Rooms, Workspace)  
* **Filtration Stages:** Pre-Filter \+ Nano Protect HEPA Filter \+ Carbon Filter  
* **Smart Features:** Sleep Mode, Real-time AQI display, PM2.5 numerical reading, Long-lasting filters (up to 3 years)  
* **Price Range:** ₹22,000 – ₹32,000

**Dyson Purifier Big+Quiet (Hot+Cool Gen1)**

* **Coverage Area:** 400–650 sq. ft. (Living rooms, Small Conferences, Bedrooms)  
* **Filtration Stages:** HEPA H13 Filter \+ Activated Carbon \+ Formaldehyde Filter  
* **Smart Features:** Night Mode, Real-time AQI value, 350° Oscillation & Air Projection  
* **Price Range:** ₹33,000 – ₹68,000

**Honeywell Air Touch U2**

* **Coverage Area:** 235–1000 sq. ft. (Home & Office Purifiers, Car Purifiers)  
* **Filtration Stages:** Anti-Bacterial Filter (Silver Ion) \+ Anti-H1N1 Layer \+ H13 HEPA Filter \+ Cold Catalyst \+ Activated Carbon Filter  
* **Smart Features:** Purifies air every 12 mins, Real-time AQI display, 9000 hrs filter life, Alexa control, WiFi \+ Smart app control  
* **Price Range:** ₹5,000 – ₹28,000

**Blue Star AP700DAI**

* **Coverage Area:** 299–915 sq. ft. (Home Purifiers)  
* **Filtration Stages:** High-Density Pre-Filter \+ H13 HEPA Filter \+ Active Carbon Filter \+ Microbe DeActive Filter (Deactivates airborne microbes)  
* **Smart Features:** Real-time AQI display, Filter change alert, Child lock, Sleep mode  
* **Price Range:** ₹8,000 – ₹27,000

### **What is the relationship between a city’s population size and its average AQI — do larger cities always suffer from worse air quality? (Consider 2024 population and AQI data for this)**

As the population increases most of the states have maintained AQI below 150\. Except Delhi its population is upto 13K and shows high AQI levels.  
In spite of Delhi having adopted EV fuels there must be a lack of implementation of the plan. 

The states of like Arunachal Pradesh, Meghalaya, Puducherry, Nagaland and Sikkim \- have greenery sites and their population is within 10k 

While other tier 1 and metro cities have populations of more than 1 Million there is an increase in AQI levels but stays within 100 to 170\.

### **How aware are Indian citizens of what AQI (Air Quality Index) means and do they understand its health implications?**

| Apps  | Ratings | Reviews  | Downloads |
| :---- | :---- | :---- | :---- |
| Sameer India's AQI | 2.7 | 1.59K | 1L+ |
| PureLogic Labs AQI app | 3.8 | 980 | 1L+ |
| IQ Air Visual | 4.6  | 3.23L | 50L+ |

Google Trends- 
1. [Term: Todays AQI](https://trends.google.com/trends/explore?cat=63&geo=IN&q=Today%20AQI&hl=en-GB)   
2. [Term: AQI near me](https://trends.google.com/trends/explore?geo=IN&q=air%20quality%20near%20me)  
     
As per the problem statement the term AQI search in India was increased when a biotech entrepreneur bryan johnson has left the podcast mid way due to bad AQI. Due to which there is a surge in the web for term AQI.  
Related queries users have searched   
* weather aqi  
* aqi delhi today  
* air quality index delhi  
* what is aqi in weather  
* imd  
* highest aqi ever recorded  
* aqi of my location  
* aqi near me

### **Which pollution control policies introduced by the Indian government in the past 5 years have had the most measurable impact on improving air quality and how have these impacts varied across regions or cities?**

***National Clean Air Program by Indian Government***

**Source: [Goverment of Indian PIB](https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=1909910)**

The Ministry of Environment, Forest and Climate Change (MoEFCC) launched the National Clean Air Programme (NCAP) in January, 2019\.   
Its aim was to improve air quality in 131 cities (non-attainment cities and Million Plus Cities) in 24 States/UTs by engaging all stakeholders.   
The programme goal was to achieve reductions up to 40% or achievement of National Ambient Air Quality Standards for Particulate Matter10 (PM 10\) concentrations by 2025-26.

| State | Annual Average PM10 Concentration (2019-2020)  | Actual Annual Average PM10 (2021 \- 2022\) |
| :---- | :---- | :---- |
| Delhi | 178 | 184 |
| Meghalaya | 98 | 183 |
| Uttar Pradesh | 197.2 | 144.5 |
| Jammu & Kashmir | 134 | 126 |
| West Bengal | 100 | 125.5 |
| Uttarakhand | 142.33 | 123 |
| Bihar | 101.5 | 120 |
| Rajasthan | 127.5 | 116 |
| Punjab | 102.29 | 97.14 |
| Orissa | 100.29 | 92.29 |
| Chandigarh | 88 | 92 |
| Madhya Pradesh | 83 | 87 |
| Himachal Pradesh | 77.29 | 77.29 |
| Assam | 72.8 | 76 |
| Telangana | 72 | 74.5 |
| Nagaland | 81.5 | 72.5 |
| Maharashtra | 80.11 | 70.11 |
| Tamil Nadu | 84 | 67 |
| Karnataka | 73.67 | 65.33 |
| Chhattisgarh | 47 | 60 |
| Andhra Pradesh | 59.45 | 59.18 |

***XV Finance Commission Air Quality Grant Scheme***

**Source:** [Link](https://www.pib.gov.in/PressReleaseIframePage.aspx?PRID=2002614#:~:text=16539%20crores%20has%20been%20allocated,are%20provided%20at%20Annexure%20%E2%80%93I.)  
**Funds Allocation:** ₹16,539 crores allocated to 42 Million Plus Cities (MPCs) (including 7 Urban Agglomerations) for the period FY 2020–21 to FY 2025–26.  
**Purpose:** To implement City Specific Action Plans (CAPs) under the National Clean Air Programme (NCAP) for performance-based air quality improvement.  
**Utilization Monitoring:**

* City-wise utilization of funds tracked and provided in Annexure–I.  
* Includes details of non-utilization by non-attainment cities.

**Resource Convergence:**  
 Implementation of CAPs is also supported through convergence with other urban schemes, such as:

* Swachh Bharat Mission (Urban)  
* AMRUT (Atal Mission for Rejuvenation and Urban Transformation)  
* Smart City Mission  
* SATAT (Sustainable Alternative Towards Affordable Transportation)  
* FAME II (Faster Adoption and Manufacturing of Hybrid and Electric Vehicles)

