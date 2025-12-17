# EDE 2025-2026 Semester Project

Date: 16.12.2025

## General Project Goals
- Carry out a data project in a student team  applying data analysis methods
- Your goal is to create a regression model for a specific project
- Organize the data and your team indepently

## Projects

All projects share the same tasks and parts, as follows:

### Part 1: Exploratory Data Analysis and Correlation Analysis
- Explore your data graphically and statistically 
    - Be concise and include focussed information and insights with your plots and diagrams
    - Focus to what's essential for understanding your data set and the model of part 2.
    - Analyse the correlation between your target variable and the other parameters

### Part 2: Train and Evaluate a Linear Regression Model

- Create a **linear regression model** for your target variable

#### Model Requirements
- Compare **at least five different regression models** with varying model complexity and different variables used, from single-feature to multi-feature models
- You may:
  - Test different feature sets
  - Engineer new features using available variables 
- Apply a **systematic approach** to identify the most relevant features for a balanced bias-variance trade-off.
- Take measures to **avoid overfitting**, e.g. by using **k-fold cross-validation**
- Visually compare your models by adequate plots 

#### Final Model Evaluation, Selection and Description
- Select the **best-performing model** and explain the **reasons for selecting** this model over alternative
- Describe the **final model**, its **structure**, its **goodness of fit**



## Project Deliverables:
**Files to upload:**
- **Jupyter Notebook**
    - **Functional Code**: The code must run on the instructor’s computer without modification
    - **Documentation in Markdown**: See evaluation criteria for documentation requirements
    - Ideally a single file
- **Source Files** (only if you manually change them)
- **HTML Version of the Notebook** (just in case)

## Project Presentation
- Maximum of **15 minutes per team**
- **All team members must present equally**
- Focus on **results and methods**, not on code
- You might also add background information to your data set, technology or system, so that everyone knows what you are presenting.
- You do **not** need to present everything; emphasize **highlights and what's relevant**
- Structure your notebook, and hide irrelevant parts, so that the presentation is not bloated.
- **No additional documents or slides** - use the **notebook only**

## Evaluation Criteria

### Submitted Notebooks
- ✅ Correctness  
- ✅ Completeness  
- ✅ Conciseness  
- ✅ Creativity of solutions  
- ✅ Programming style  
- ✅ Code documentation  
- ✅ Application of theory and methods  

### Documentation 
- Appendix to Notebook required, which consists of:

#### Contribution of student 
Clearly make contribution per student transparent: who contributed what? Who was working on which task?
e.g.
- **Student 1:**: x, y, z (xx %)
- **Student 2:**  z (xx%), B, A

#### Sources
- List all external sources (papers, websites, libraries, AI tools, etc.)
- AI assistance, Coding assistants and LLMs usage is generally **allowed**
- Usage must be made **transparent**
- Clearly describe:
  - **When** AI was used
  - **How** AI contributed (e.g., idea generation, debugging, documentation)

### Grading
- Individual grade for group project
- Individual grade for presentation
- Individual grade for oral examination



## Individual Team Projects

Each student team is working on different projects, to be selected from the following list:

### Project 1: Solar Thermal Collector

Dataset: 
- FHW_ArcS__main__2017_resampled.csv (Resampled to 15 min time steps and removed standard deviation)

Meta data: 
- solar_thermal/FHW_ArcS__parameters.json

Objective: 
- Predict solar thermal collector output Y: 'tp__calc'
- Allowed regressor variables X: 'vf', 'mf__calc', , 'te_in',  'rho_in__calc',
       'rho_out__calc', 'cp_in__calc', 'cp_out__calc', 'rd_gti', 'rd_ghi',
       'rd_bti__calc', 'rd_bhi__calc', 'rd_dni', 'rd_dti__calc',
       'rd_dhi__calc', 'te_amb', 've_wind', 'rh_amb', 'aoi__calc',
       'sun_azimuth__calc', 'sun_apparent_elevation__calc',
       'is_shadowed__calc', 'is_shadowed_external',
       'rd_bti_shadowed_share__calc', 'is_shadowed_internal__calc'
- Excluded regressor variables: 'te_out', 'te_out_row1',
       'te_out_row2', 'te_out_row3', 'te_out_row4',

Sources: 
- Dataset: https://zenodo.org/records/7741084
- Article: https://doi.org/10.1016/j.dib.2023.109224


### Project 2: Air Source Heat Pump

Dataset: 
- "EOH0669.csv", corresponds to Property_ID

Meta Data:  
- "DESNZ Electrification of Heat Project - Heat Pump Performance Data Summary.csv"

Objective: 
- Calculate COP: COP = Heat_Pump_Energy_Output / Whole_System_Energy_Consumed
- Predict Y: COP
- Allowed regressor variables X: Circulation_Pump_Energy_Consumed,Heat_Pump_Energy_Output,External_Air_Temperature,Heat_Pump_Heating_Flow_Temperature,Heat_Pump_Return_Temperature,Internal_Air_Temperature,Hot_Water_Flow_Temperature,
- Excluded regressor variables: Whole_System_Energy_Consumed, Immersion_Heater_Energy_Consumed,Back-up_Heater_Energy_Consumed

Sources: 
- Raw data: https://datacatalogue.ukdataservice.ac.uk/studies/study/9209
- Meta Data: https://usmart.io/org/esc/discovery/discovery-view-detail/6a5e5753-aaff-455e-8b3b-8ee282010261
    - "DESNZ Electrification of Heat Project - Heat Pump Performance Data Summary.csv"
- Project Reports: https://es.catapult.org.uk/report/electrification-of-heat-summary-reports-and-datasets

### Project 3: Ground Source Heat Pump

Dataset: 
- "EOH0451.csv", corresponds to Property_ID

Meta Data: 
- "DESNZ Electrification of Heat Project - Heat Pump Performance Data Summary.csv"

Objective:
- Calculate COP: COP = Heat_Pump_Energy_Output / Whole_System_Energy_Consumed
- Predict Y: COP
- Allowed regressor variables X: Circulation_Pump_Energy_Consumed,Heat_Pump_Energy_Output,External_Air_Temperature,Heat_Pump_Heating_Flow_Temperature,Heat_Pump_Return_Temperature,Internal_Air_Temperature,Hot_Water_Flow_Temperature,Brine_Flow_Temperature,Brine_Return_Temperature

- Excluded regressor variables: Whole_System_Energy_Consumed, Immersion_Heater_Energy_Consumed,Back-up_Heater_Energy_Consumed

Sources: 
- Raw data: https://datacatalogue.ukdataservice.ac.uk/studies/study/9209
- Meta Data: https://usmart.io/org/esc/discovery/discovery-view-detail/6a5e5753-aaff-455e-8b3b-8ee282010261
    - "DESNZ Electrification of Heat Project - Heat Pump Performance Data Summary.csv"
- Project Reports: https://es.catapult.org.uk/report/electrification-of-heat-summary-reports-and-datasets


### Project 4: Onshore Wind Turbine

Dataset: 
- "Inland Wind Farm Dataset1(WT1).csv"

Metadata:
- https://zenodo.org/records/5516552

Objective: 
- Calculate power output: P_turbine = y (% relative to rated power)*P_nominal
    P_nominal = 1.5 MW
- Predict Y: P_turbine
- Regressor Variables: V: wind speed; D: wind direction; rho: air density; H: humidity; I: turbulence intensity; Sb: below-hub height wind shear

Sources: 
- Data: https://zenodo.org/records/5516552
- Ding: Data Science for Wind Energy, https://aml.engr.tamu.edu/book-dswe/



### Project 5: Offshore Wind Turbine

Dataset: "Offshore Wind Farm Dataset1(WT6).csv"

Metadata: https://zenodo.org/records/5516552

Objective: 
- Calculate power output: P_turbine = y (% relative to rated power)*P_nominal
    P_nominal = 3.0 MW
- Predict Y: P_turbine
- Regressor Variables: V: wind speed; D: wind direction; rho: air density; H: humidity; I: turbulence intensity; S: vertical wind shear; Sa: above-hub height wind shear, Sb: below-hub height wind shear


Sources: 
- Data: https://zenodo.org/records/5516552
- Ding: Data Science for Wind Energy, https://aml.engr.tamu.edu/book-dswe/


### Project 6: Small-scale PV system

Dataset: "station00.csv"

Metadata: https://doi.org/10.11922/sciencedb.01094

Objective: 
- Predict: power
- Regressor variables: nwp_globalirrad,nwp_directirrad,nwp_temperature,nwp_humidity,nwp_windspeed,nwp_winddirection,nwp_pressure,lmd_totalirrad,lmd_diffuseirrad,lmd_temperature,lmd_pressure,lmd_winddirection,lmd_windspeed

Sources:
- Data: PVOD v1.0 : A photovoltaic power output dataset, https://doi.org/10.11922/sciencedb.01094
- Paper: https://doi.org/10.1016/j.solener.2021.09.050


### Project 7: Large-scale PV System

Dataset: "station05.csv"

Metadata: https://doi.org/10.11922/sciencedb.01094

Objective: 
- Predict: power
- Regressor variables: nwp_globalirrad,nwp_directirrad,nwp_temperature,nwp_humidity,nwp_windspeed,nwp_winddirection,nwp_pressure,lmd_totalirrad,lmd_diffuseirrad,lmd_temperature,lmd_pressure,lmd_winddirection,lmd_windspeed

Sources:
- Data: PVOD v1.0 : A photovoltaic power output dataset, https://doi.org/10.11922/sciencedb.01094
- Paper: https://doi.org/10.1016/j.solener.2021.09.050


### Project 8: Heating power UMAR

Dataset: 
- "umar_2019_2022_resampled.csv" (Resampled to 15 min time steps and merged)

Metadata: 
- "umar_metadata.csv"

Objective: 
- Predict: heating_power
- Regressor variables: 
irrad,setp_272,setp_273,setp_274,setp_275,setp_276,temp_272,temp_273,temp_274,temp_275,temp_276,temp_amb,total_active_power,window_272,window_273_1,window_273_2,window_274,y1_272,y1_273,y1_274,y1_275,y1_276,y2_273,y3_273
- Excluded variables: time, cooling_power, dhw_power,dhw_volume

Sources:
- Heer, Philipp (2024). NEST Open Building Data for Energy Demand and User Practice. figshare. Collection. https://doi.org/10.6084/m9.figshare.c.7178787.v1 
- Paper: https://www.nature.com/articles/s41597-024-03292-2

### Project 9: Heating and cooling power DFAB

Dataset: 
- "dfab_2019_2022_resampled.csv" (Resampled to 15 min time steps and merged)

Metadata: 
- "dfab_metadata.csv"

Objective: 
- Predict: heating_cooling_power
- Regressor variables: irrad	kitchen_active_power	setp_371	setp_472	setp_474	setp_476	setp_571	setp_573	setp_574	shower_471	shower_571	temp_371	temp_472	temp_474	temp_476	temp_571	temp_573	temp_574	temp_amb	total_active_power	
- Excluded variables (valve settings): y1_371	y1_472	y1_474	y1_476	y1_571	y1_573	y1_574	y2_371	y2_472	y2_476	y2_571	y2_574	y3_371	y3_472	y3_476	y3_571	y3_574	y4_371	y5_371	y6_371	y7_371

Sources:
- Heer, Philipp (2024). NEST Open Building Data for Energy Demand and User Practice. figshare. Collection. https://doi.org/10.6084/m9.figshare.c.7178787.v1 
- Paper: https://www.nature.com/articles/s41597-024-03292-2

### Project 10: Cooling power SolAce

Dataset: 
- "solace_2019_2022_resampled.csv" (Resampled to 15 min time steps and merged)

Metadata: 
- "solace_metadata.csv"

Objective: 
- Predict: cooling_power
- Regressor variables: 
blinds_angle_F1	blinds_angle_F2	blinds_height_F1	blinds_height_F2	blinds_height_F3	blinds_height_F4	irrad	praes_meeting	praes_office	pv_active_power	setp_meeting	setp_office	temp_amb	temp_meeting	temp_office	total_active_power	
- Excluded variables heating_power  y1_meeting	y1_office

Sources:
- Heer, Philipp (2024). NEST Open Building Data for Energy Demand and User Practice. figshare. Collection. https://doi.org/10.6084/m9.figshare.c.7178787.v1 
- Paper: https://www.nature.com/articles/s41597-024-03292-2
