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
    - High Corlation with:
      - ```wind_speed```(0.23)
      - ```precip_depth_1_hr```(0.12)
      - ```dew_temperature```(0.15)
      - ```year_built```(0.18)
      - ```site_id```(-0.24)
      - ```building_id```(-0.25)
      - ```meter```(-0.18)
  - dew_temperature        0.50%
  - precip_depth_1_hr     18.54%
    - High Corlation with:
      - ```cloud_coverage```(0.12)
  - sea_level_pressure     6.09%
    - High Corlation with:
      - ```air_temperature```(-0.48)
      - ```building_id```(0.16)
      - ```site_id```(0.13)
      - ```year_built```(-0.14)
      - ```dew_temperature```(-0.26)
      - ```wind_speed```(-0.16)
  - wind_direction         7.17%
    - High Corlation with:
      - ```dew_temperature```(-0.19)
      - ```wind_direction```(0.5)
  - wind_speed             0.71%
  
 ## Other Nots:
   - ```DT_day_week``` range from 0 to 6, 0 is Sunday and 6 is Saturday
   - Group wind in to N,NE,E,SE,S,SW,W,NW
     - N  = 337.5-22.5
     - NE = 67.5
     - E  = 112.5
     - SE = 157.5
     - S  = 202.5
     - SW = 247.5
     - W  = 292.5
     - NW = 337.7