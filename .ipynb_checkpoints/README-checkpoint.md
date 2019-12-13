# ashrae-energy  
## Potential Features  
  - Average floor area
  - Is workday
  
## Categorical  
  - One-Hot Encoding  
      - ```primary_use```
      - ```meter```
      

## Highly Corlated Features  
  - ```dew_temperature```, ```air_temperature``` 0.72
  - ```sea_level_presure```, ```air_temperature``` -0.47
  - ```wind_direction```, ```wind_speed``` 0.47
  - ```meater```, ```building_id``` 0.22 *beore building_id is encoded* 

## Contains Missing Values  
  - air_temperature        0.48%
  - cloud_coverage        43.66%
  - dew_temperature        0.50%
  - precip_depth_1_hr     18.54%
  - sea_level_pressure     6.09%
  - wind_direction         7.17%
  - wind_speed             0.71%
  
