# Water Activities Dashboard for Houston Area

## Premise

As someone who has a paddle board, whitewater kayak, and sea kayak who often takes them to local rivers, 
lakes, bays, and surf in the Houston area, I frequently check several different sources of online 
information to determine what potential trips are possible given the conditions. 

Going to several different sites is a bit slow. Some of them are apps and others are just webpages I have 
saved to my phone in a folder. 

It would save me time, if I could create a website that collects all the information in one place that lets
me decide what water activities are possible for a given upcoming day.

## Data Sources
- Surfline (app or website)
- Magic Seaweed (app or website)
- Web cam of Buffalo Bayou (website)
- USGS water guage of Buffalo Bayou at Shepard Drive (website)
- USGS water guage of Buffalo Bayou at Piney Point (website)
- Weather site (app or website)
- Lightning Map (website)

## Information Types
- River levels
- River flow velocity
- Wind speed
- Wind direction
- Timing of changes in wind direction
- Rain forecast
- Lightning forecast
- Radar imagery
- Surf height
- Swell height
- Swell direction
- Tides


## Information Time Periods
- Several days ahead
- By hours within a given day

## Decision Point Metrics
With first guesses at decision point scenarios
- Lightning forecast probability > 30% a day ahead for for all activities
- Lightning < 100 miles for all activities
- Wind speed > 16mph for paddle boarding by myself
- Wind speed >12mph for paddle boarding with others
- Wind speed > 18 mph for sea kayaking myself in bay or other exposed water
- Wind speed > 20 mph for river kayaking 
- Wind speed > 20 mph for river kayaking 
- Surf height > 5 feet for sea kayaking 
- Surf height < 1 feet for surf paddle boarding
- Swell quality indicator == red

## Questions for Building Proof of Concept
- Can all sites be embedded? 
  - What sites can't? 
  - Do they have APIs?
- What would save time beyond just having all the links to click in one spot?
- What's the right mix of buttons that link, embeds, APIs used that builds data visualizations?
- Templates that serve this need or scratch or framework?
- Just front-end or any need for a backend?
- Any benefits from saving data, conditions, or experiences?
  - For buffalo bayou:
    - Give height and past experience:
        - bi-directional trips from single put-in/take-out won't work as river is too high
        - too fast to take others
        - river has been too high by X amount for X days
        - map our times of year river has historically been too high for bi-directional or even one-way trips based on different skill levels



## Doodles

#### First draft
https://observablehq.com/d/23f79d02e6033913


Buffalo Bayou API call example: 

https://nwis.waterservices.usgs.gov/nwis/iv/?format=json&sites=08074000&startDT=2017-06-01&endDT=2021-06-03&parameterCd=00060,00065&siteStatus=all

Generated from this page: 

https://waterservices.usgs.gov/rest/IV-Test-Tool.html


#### USGS Plot Code
Looked at this, but it doesn't look like I can control how far down the fill occurs or add a datum line at a given value
https://txpub.usgs.gov/dss/gwis/0.0/doc/#documentation

## Possible Organizational Structure For Trips


### What should be top-level organizing variable?

#### Possibilities

##### Description of possible trip

- body_of_water: ""
  - trip_name: ""
  - put_in: ["latitude":"","longitude":""]
  - take_out: ["latitude":"","longitude":""]
  - put_in_name: ""
  - take_out_name: ""
  - one_way_or_come_back_to_start:""
  - activity_types_possible:[]
  - boat_type_best_for_this_location:""
  - paddler_skill_level_from_enum_possible:[""]
  - trip_difficulty_description:""
  - paddler_minimum_skill_level:""
  - whitewater_class:""
  - water_if_moving_range:[""]
  - tidal_range_that_is_best:[integer]
  - link_to_tidal_forecast:""
  - link_to_river_gage_nearest:""
  - gage_level_max_for_skill_and_boat_level_high:""
  - gage_level_max_for_skill_and_boat_level_average:""
  - gage_level_max_for_skill_and_boat_level_low:""
  - wind_an_issue_boolean:""
  - wind_direction_worst_for_this_trip:""
  - wind_direction_best_for_this_trip:""
  - surfing_shoreline_orientation:""
  - surfing_wave_best_orientation:""

##### Details of actual trip

same as above, plus:

- trip_name_actual: ""
- boat_type_used_on_trip_from_enum:""
- boat_type_used_on_trip_description:""
- activity_type:""
- paddler_skill_level_from_enum_actual:[]
- trip_difficulty_description_actual:""
- whitewater_class:""
- tide_actual:""
- date_trip_started:""
- date_trip_ended:""
- time_time_trip_started:""
- time_time_trip_ended:""
- wind_speed_actual:""
- wind_direction_actual:""
- surf_height_actual:""
- surf_period_actual:""
- surf_quality_actual:""