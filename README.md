This is the Resume Project Challenge for conducting a product market fit analysis on air purifiers. This challenge is powered by Codebasics platform and sponsored by dataful platform.


##  *<p align="center">Problem Statement</p>*


According to the IQ air reports around the world there are 20 air polluted urban cities which have higher AQI index out of which 14 cities are from India.

To tackle with this AirPure Innovations is a startup born out of the air quality crisis in India. The company is in the early stages of the product development and is unsure whether there is a strong, sustained demand for its air purifier product.

 They want to understand the patterns of the AQI across Indian states before committing to Production and R\&D by answering the critical questions: 

1. What pollutants or particles should their air purifier target?  
2. What are the most essential features that should be incorporated into the air purifier?  
3. Which cities have the highest demand for air purifiers, and what is the market size in these regions?  
4. How can R\&D be aligned with localized pollution patterns?

##  *<p align="center">Dataset Information</p>*

### **Dataset: Day-wise, State-wise Air Quality Index (AQI) of Major Cities and Towns in India**

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

### **Dataset: State, District, and Disease-wise Cases and Deaths reported due to Outbreak of Diseases as per Weekly reports under IDSP**

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

### **Dataset: State, Vehicle Class and Fuel Type-wise Total Number of Vehicles Registered in Each Month in India**

This dataset contains monthly records of the number of vehicles registered in India, categorized by state, vehicle class (e.g., two-wheeler, car, bus), and fuel type (e.g., petrol, diesel, electric). It provides insights into vehicle registration trends across different states and fuel categories over time.

**Time Coverage:** Monthly coverage from year 2022 till 2025

| Column Name | Data Type | Description |
| ----- | ----- | ----- |
| State | Text | Name of the Indian state where the vehicles were registered |
| Month | Text / Date | Month and year of vehicle registration (e.g., Jan-2023) |
| Vehicle Class | Text | Category/type of vehicle (e.g., Two-Wheeler, LMV, HMV, Bus, etc.) |
| Fuel Type | Text | Type of fuel the vehicle uses (e.g., Petrol, Diesel, Electric, CNG) |
| Number of Vehicles | Numeric | Total number of vehicles registered under the given category in that month |

### **Dataset: Population Projection of India: State- and Gender-wise Yearly Projected Urban Population (2011-2036)**

This dataset provides projected urban population figures for Indian states, disaggregated by gender (male and female) for each year from 2011 to 2036\. These projections are based on estimates from official census data and demographic models, and are intended for use in urban planning, resource allocation, and policy formulation.

**Time Coverage:** From year 2011 \- 2036 monthly data.

| Column Name | Data Type | Description |
| ----- | ----- | ----- |
| State | Text | Name of the Indian state |
| Year | Numeric | Year of the projected population (ranging from 2011 to 2036\) |
| Male Population | Numeric | Projected urban male population for the specified state and year |
| Female Population | Numeric | Projected urban female population for the specified state and year |
| Total Population | Numeric | Sum of projected male and female urban population for that state and year |

##  *<p align="center">Primary Questions</p>*

#### **List the top 5 and bottom 5 areas with highest average AQI. (Consider areas which contains data from last 6 months: December 2024 to May 2025\)**

**Bottom 5 areas**
It shows areas with lowest AQI, Tirunelveli has one of the lowest AQI of 33.31.

In the top 5 areas it shows Byrnihat (Meghalaya) with 284.19 AQI, Delhi as the second position with 238.92.   
The reason for **Byrnihat on top is due to its industrialization environment.** There are many industries of machinery, distillery, cement and steel. Also its geographical environment location on the Assam-Meghalaya border, with its unique topography, consists of a low pressure zone which traps pollutants and makes it unable to disperse.

**Reasons for High AQI Levels** 
- Seasonal stubble Burning in agricultural areas   
- Industrial activity  
- Geographical location factor low air pressure which can trap pollutants in air  
- Constructions and vehicular emission

The AQI in Chamarajanagar, Vijayapura, Madikeri (Karnataka), and Tirunelveli (Tamil Nadu), including the border area of Palkalaiperur, is likely low due to a combination of factors such as **lower industrial activity, less population density, and potentially more green cover**. These areas are not major industrial hubs and have a relatively smaller population compared to larger cities, which contributes to better air quality.

<img width="800" height="417" src="https://github.com/user-attachments/assets/d8e857ba-6703-4b02-b4ba-93818372b094" />

#### **List out top 2 and bottom 2 prominent pollutants for each state of southern India.  (Consider data post covid: 2022 onwards)**

PM10 and PM2.5 stand out as the top pollutants across southern states while few other pollutants such NH3, NO2, O3, and SO2. The factors could be more number of vehicles, construction and demolition, duct and debris. 

<img width="800" height="360" alt="image" src="https://github.com/user-attachments/assets/52507248-930d-4d03-9d10-13e562a53883" />

#### **Does AQI improve on weekends vs weekdays in Indian metro cities (Delhi, Mumbai, Chennai, Kolkata, Bengaluru, Hyderabad, Ahmedabad, Pune)?(Consider data from last 1 year)**

There is a slight drop of AQI from March to May ( due to holiday season ), August to October and December. Since in these months most people either go for a vacation, and other seasonal factors.

**Insights based on the Monthly chart of each states**   
It shows months from April to mid \- October and seasonal time for monsoon where AQI has a sudden drop which is normal for every state.
During the month of Oct \- Jan the AQI is at its peak the factors could be harvesting seasonal in which stubble burning is done around those states. 

<img width="800" height="450" alt="image" src="https://github.com/user-attachments/assets/ee3c5fc8-e1c7-4b20-b53f-337a7fa99399" />

#### **Which months consistently show the worst air quality across Indian states (Consider top 10 states with high distinct areas)**

Months of January, February and December show signs of high AQI. While November is a leading month in most all those states. 

Months ranging from Mid-April or May till September we can see there is a sudden drop of the AQI for this a dominant factor can be a monsoon season. 

After the monsoon season, harvesting seasons start for various states in different timelines so we can see there is a rise of AQI level from October till Jan and more or less it can expand till April. Depends on the state's geographical location.

As we see in the line chart there is only a slight difference between weekday and weekend AQI levels.

<img width="800" height="650" alt="image" src="https://github.com/user-attachments/assets/30567ea7-adbb-4b6a-b404-4f9dbccc9234" />

#### **For the city of Bengaluru, how many days fell under each air quality category (e.g., Good, Moderate, Poor, etc.) between March and May 2025?**

In the Pie chart we see that Bengaluru has 13 days with moderate level AQI and 48 days with Satisfactory level AQI. 

<img width="600" height="502" alt="image" src="https://github.com/user-attachments/assets/1537e28b-31ee-402c-a6b7-bf113afcefbf" />

#### **List the top two most reported disease illnesses in each state over the past three years, along with the corresponding average Air Quality Index (AQI) for that period.**

Based on the reports of the table we can see two most prominent diseases are Acute Diarrheal Disease and Food Poisoning. 

Kerala, Maharashtra, Karnataka, Odisha, Chhattisgarh tops the chart with more disease cases. In terms of AQI Delhi, Jharkhand, Himachal Pradesh, Bihar, Chandigarh tops the list having highest AQI in the past 3 years but their disease cases are not that correlated with the AQI levels.

<img width="800" height="672" alt="image" src="https://github.com/user-attachments/assets/a8c29f6d-a552-43f1-8f21-b5055421b3d4" />

#### **List the top 5 states with high EV adoption and analyse if their average AQI is significantly better compared to states with lower EV adoption.**

The EV fuels selected are Electric (BOV), Fuel Cell Hydrogen, Plug-in Hybrid EV, Pure EV, Solar and Strong Hybrid EV. 

Uttar Pradesh, Maharashtra, Karnataka, Tamil Nadu and Rajasthan rank as the top 5 states with High EVs registration. Their overall average AQI is 101.27 which is pretty less than the overall average AQI of other states which is 119.53. It can be the reason that EVs have played a better role in reducing AQI levels. 

<img width="800" height="691" alt="image" src="https://github.com/user-attachments/assets/196b0c6e-c930-41df-a730-3a51c2d8a5a4" />

##  *<p align="center">Secondary Questions</p>*

#### **Which age group is most affected by air pollution-related health outcomes and how does this vary by city?**

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

#### **Who are the major competitors in the Indian air purifier market, and what are their key differentiators (e.g., price, filtration stages, smart features)?**

#### Air Purifier Competitor Matrix  

| Brand          | Price Range (INR) | Coverage Area (sq.ft) | Filtration Stages                                                                                       | Category                                      | Smart Features                                                                                                   | Alerts to change Filters | App Access | Quiet Mode | Voice Control | VOCs | Real Time AQI |
|----------------|------------------|------------------------|---------------------------------------------------------------------------------------------------------|-----------------------------------------------|------------------------------------------------------------------------------------------------------------------|--------------------------|------------|------------|---------------|------|----------------|
| **Dyson**      | 33K - 68K        | 400 - 1000            | Evo Carbon Filter, 360° Glass HEPA 13, Carbon Air Purifier Filter, Formaldehyde Filter                  | Living Rooms, Small Conferences, Bedroom      | Remote Control, Quieter Sound (56dBA), App Access, Auto Mode, Voice Control (Siri, Alexa, Google), Night Mode, VOCs Indicator | ✅                        | ✅          | ✅          | ✅             | ✅    | ✅              |
| **Philips**    | 8K - 15K         | 300 - 1000            | HEPA Filter, Active Carbon Filter, Pre-Filter                                                           | Large, Medium, Small, Compact Areas           | App Connectivity, Ultra Quiet Mode, Real Time AQI Display, PM2.5 Sensor, Voice Control (Alexa, Google Home)       | ✅                        | ✅          | ✅          | ✅             | ❌    | ✅              |
| **Eureka Forbes** | 1K - 19K      | 200 - 500             | Pre-Filter, Activated Carbon Filter, True H13 HEPA Filter, Plasma Filter                                | Quick Cleaning, Bedrooms, Living Rooms (480 sq.ft.) | WiFi Enabled, PM2.5 Digital Display, 360° Air Intake, Real Time AQI, Quiet Mode, VOCs Indicator, Child Lock        | ✅                        | ✅          | ✅          | ❌             | ✅    | ✅              |
| **Honeywell**  | 5K - 28K         | 235 - 1000            | Pre-Filter, Anti-Bacterial Filter (Silver Ion), Anti H1N1 Layer, H13 HEPA, Cold Catalyst, Activated Carbon | Home & Office Purifiers, Car Purifiers        | Purifies Air Every 12 mins, Real Time AQI Display, 9000 Hrs Filter Life, Voice Control (Alexa), WiFi + App, Child Lock, VOCs Indicator | ✅                        | ✅          | ✅          | ✅             | ✅    | ✅              |
| **Blue Star**  | 8K - 27K         | 299 - 915             | Pre-Filter, H13 HEPA, Activated Carbon, Microbe DeActive Filter                                         | Home Purifiers                                | Real Time AQI, Child Lock, Sleep Mode, VOC Sensor, PM2.5 Indicator, Touch Interface                               | ✅                        | ❌          | ❌          | ❌             | ✅    | ✅              |
| **Coway**      | 20K - 59K        | 355 - 930             | Pre-Filter, True H13 HEPA, Deodorization Filter                                                         | Home Purifiers                                | 360° Air Purification, Real Time AQI, Remote Control, Auto Oscillation (80°)                                     | ✅                        | ❌          | ❌          | ❌             | ✅    | ✅              |

#### **What is the relationship between a city’s population size and its average AQI — do larger cities always suffer from worse air quality? (Consider 2024 population and AQI data for this)**

<img width="600" height="450" alt="image" src="https://github.com/user-attachments/assets/1c3fce98-e14a-4487-bc2d-0e8e5acb3759" />

As the population increases most of the states have maintained AQI below 150\. Except Delhi its population is upto 13K and shows high AQI levels.  
In spite of Delhi having adopted EV fuels there must be a lack of implementation of the plan. 

The states of like Arunachal Pradesh, Meghalaya, Puducherry, Nagaland and Sikkim \- have greenery sites and their population is within 10k 

While other tier 1 and metro cities have populations of more than 1 Million there is an increase in AQI levels but stays within 100 to 170\.

#### **How aware are Indian citizens of what AQI (Air Quality Index) means and do they understand its health implications?**

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

#### **Which pollution control policies introduced by the Indian government in the past 5 years have had the most measurable impact on improving air quality and how have these impacts varied across regions or cities?**

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

##  *<p align="center">Final Analysis</p>*

Based on research done the air purifier market and products below shows 3 prototypes of that can be develop. 


#### Air Purifier Segmentation (Basic vs Medium vs Premium)

For Tier 1 cities Basic and Medium plans can be pitched and for tier 2 cities medium and premium plans.

| Feature / Category      | Basic             | Medium              | Premium                |
|-------------------------|-------------------|---------------------|------------------------|
| **Filter Type**          | Pre-Filter, Activated Carbon Filter, True H13 HEPA Filter | Pre-Filter, Activated Carbon Filter, True H13 HEPA Filter, Microbe DeActive Filters, Anti-Bacterial Filters | Pre-Filter, Activated Carbon Filter, True H13 HEPA Filter, Microbe DeActive Filters, Anti-Bacterial Filters, VOC Filters, UV Light Filters |
| **Category**             | Small Rooms | Medium Rooms (bedrooms, halls, living areas) | Large Spaces (offices, halls, living rooms) |
| **Real Time AQI Display**| ✅  | ✅   | ✅  |
| **PM2.5 Indicator**      | ✅  | ✅  | ✅  |
| **Alerts to Change Filters** | ✅ | ✅  | ✅ |
| **Quiet Mode**           | ❌ | ✅ | ✅ |
| **Voice Control**        | ❌ | ✅ | ✅ |
| **App Access**           | ❌ | ✅ | ✅ |
| **Remote Control**       | ✅ | ✅ | ✅ |
| **Touch Screen**         | ❌ | ❌ | ✅ |
| **Child Lock**           | ❌ | ✅ | ✅ |
| **Smart AQI Syncing**    | ❌ | ❌ | ✅ |



####  <p align="center">TIER 1 CITIES </p>


| **Area**  | **Average AQI** |
| --------- | --------------- |
| Delhi     | 204.26          | 
| Ahmedabad | 111.46          |
| Pune      | 108.95          | 
| Mumbai    | 105.49          | 
| Kolkata   | 100.87          | 
| Hyderabad | 79.91           | 
| Chennai   | 73.83           | 
| Bengaluru | 73.28           | 

####  <p align="center">TIER 2 CITIES </p>

| Area            | Average AQI | Area               | Average AQI |
| --------------- | ----------- | ------------------ | ----------- |
| Aurangabad      | 119.31      | Raichur            | 93.33       |
| Akola           | 92.47       | Vijayapura         | 50.51       |
| Amravati        | 88.40       | Kannur             | 67.14       |
| Bhiwandi        | 106.35      | Kochi              | 99.98       |
| Dhule           | 104.28      | Kollam             | 78.83       |
| Jalgaon         | 109.07      | Kozhikode          | 67.37       |
| Kolhapur        | 93.27       | Thiruvananthapuram | 50.77       |
| Nagpur          | 109.19      | Thrissur           | 65.32       |
| Nanded          | 99.26       | Bhopal             | 117.77      |
| Nashik          | 80.77       | Gwalior            | 144.52      |
| Sangli          | 78.67       | Indore             | 98.74       |
| Solapur         | 95.48       | Jabalpur           | 114.85      |
| Agra            | 83.14       | Ratlam             | 100.23      |
| Bareilly        | 79.16       | Ujjain             | 125.05      |
| Ghaziabad       | 182.20      | Ajmer              | 101.28      |
| Gorakhpur       | 98.13       | Bikaner            | 158.49      |
| Jhansi          | 95.22       | Jaipur             | 130.43      |
| Kanpur          | 112.22      | Jodhpur            | 126.24      |
| Lucknow         | 128.41      | Kota               | 130.20      |
| Meerut          | 161.62      | Vijayawada         | 72.53       |
| Moradabad       | 105.86      | Visakhapatnam      | 114.93      |
| Noida           | 187.36      | Patna              | 179.22      |
| Prayagraj       | 95.05       | Amritsar           | 124.84      |
| Varanasi        | 67.55       | Jalandhar          | 111.60      |
| Coimbatore      | 68.87       | Ludhiana           | 131.12      |
| Madurai         | 47.93       | Patiala            | 103.73      |
| Salem           | 73.04       | Faridabad          | 186.00      |
| Thanjavur       | 41.93       | Karnal             | 108.82      |
| Tiruchirappalli | 52.01       | Dhanbad            | 174.55      |
| Tirunelveli     | 30.34       | Bhubaneswar        | 126.26      |
| Tiruppur        | 75.78       | Cuttack            | 124.69      |
| Vellore         | 69.74       | Rourkela           | 125.47      |
| Asansol         | 142.74      | Bhilai             | 71.61       |
| Durgapur        | 132.23      | Bilaspur           | 68.61       |
| Siliguri        | 79.58       | Raipur             | 77.71       |
| Surat           | 122.74      | Guwahati           | 112.90      |
| Dharwad         | 74.62       | Dehradun           | 97.56       |
| Hubballi        | 74.79       | Srinagar           | 69.50       |
| Kalaburagi      | 63.67       | Chandigarh         | 141.27      |
| Mysuru          | 50.55       | Puducherry         | 56.46       |


####  <p align="center">Priority Cities: Which Tier 1/2 cities show irreversible AQI degradation? </p>

It shows cities with worst AQI which is irreversible. 

| Area       | Average AQI | Tier Type |
| ---------- | ----------- | --------- |
| Ujjain     | 500         | Tier 2    |
| Vijayawada | 459         | Tier 2    |
| Dhanbad    | 436         | Tier 2    |
| Faridabad  | 428.79      | Tier 2    |
| Delhi      | 427.29      | Tier 1    |
| Meerut     | 424         | Tier 2    |
| Noida      | 423.22      | Tier 2    |
| Ghaziabad  | 414.88      | Tier 2    |
| Chandigarh | 412         | Tier 2    |
| Patna      | 409.63      | Tier 2    |
| Ludhiana   | 408         | Tier 2    |
| Aurangabad | 404         | Tier 2    |
| Bikaner    | 403         | Tier 2    |


####  <p align="center">Health Burden:How do AQI spikes correlate with pediatric asthma admissions? </p>

Only diseases related to asthma and respiratory conditions are considered below.
The data suggests that as AQI values increase, there can be a rise in cases of measles, diphtheria, and swine flu.
Although these diseases are not directly caused by poor air quality, it can be inferred that a polluted environment with toxic air pollutants worsens the AQI, which may contribute to increased vulnerability and severity of such diseases.

<img width="1242" height="686" alt="image" src="https://github.com/user-attachments/assets/02260a26-8b86-4278-95d2-45821a54d45a" />


