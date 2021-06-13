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
