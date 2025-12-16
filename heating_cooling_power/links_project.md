
### Project 8: Heating power UMAR

Dataset: "umar_2019_2022_resampled.csv" (Resampled to 15 min time steps and merged)
Metadata: "umar_metadata.csv"

Objective: 
- Predict: heating_power
- Regressor variables: 
irrad,setp_272,setp_273,setp_274,setp_275,setp_276,temp_272,temp_273,temp_274,temp_275,temp_276,temp_amb,total_active_power,window_272,window_273_1,window_273_2,window_274,y1_272,y1_273,y1_274,y1_275,y1_276,y2_273,y3_273
- Excluded variables: time, cooling_power, dhw_power,dhw_volume

Sources:
- Heer, Philipp (2024). NEST Open Building Data for Energy Demand and User Practice. figshare. Collection. https://doi.org/10.6084/m9.figshare.c.7178787.v1 
- Paper: https://www.nature.com/articles/s41597-024-03292-2

### Project 9: Heating and cooling power DFAB

Dataset: "dfab_2019_2022_resampled.csv" (Resampled to 15 min time steps and merged)
Metadata: "dfab_metadata.csv"

Objective: 
- Predict: heating_cooling_power
- Regressor variables: irrad	kitchen_active_power	setp_371	setp_472	setp_474	setp_476	setp_571	setp_573	setp_574	shower_471	shower_571	temp_371	temp_472	temp_474	temp_476	temp_571	temp_573	temp_574	temp_amb	total_active_power	
- Excluded variables (valve settings): y1_371	y1_472	y1_474	y1_476	y1_571	y1_573	y1_574	y2_371	y2_472	y2_476	y2_571	y2_574	y3_371	y3_472	y3_476	y3_571	y3_574	y4_371	y5_371	y6_371	y7_371

Sources:
- Heer, Philipp (2024). NEST Open Building Data for Energy Demand and User Practice. figshare. Collection. https://doi.org/10.6084/m9.figshare.c.7178787.v1 
- Paper: https://www.nature.com/articles/s41597-024-03292-2

### Project 10: Cooling power SolAce

Dataset: "solace_2019_2022_resampled.csv" (Resampled to 15 min time steps and merged)
Metadata: "solace_metadata.csv"

Objective: 
- Predict: cooling_power
- Regressor variables: 
blinds_angle_F1	blinds_angle_F2	blinds_height_F1	blinds_height_F2	blinds_height_F3	blinds_height_F4	irrad	praes_meeting	praes_office	pv_active_power	setp_meeting	setp_office	temp_amb	temp_meeting	temp_office	total_active_power	
- Excluded variables heating_power  y1_meeting	y1_office

Sources:
- Heer, Philipp (2024). NEST Open Building Data for Energy Demand and User Practice. figshare. Collection. https://doi.org/10.6084/m9.figshare.c.7178787.v1 
- Paper: https://www.nature.com/articles/s41597-024-03292-2