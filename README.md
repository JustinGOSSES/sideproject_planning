# Sideproject Planning
Side project planning to avoid just.... working on stuff

## Current Most Active Projects Are:
- [LAGADL:Large-language-model Assisted Geology Descriptions of Arbitrary Locations](https://github.com/JustinGOSSES/LAGDAL) : reusable visualizations of the community that comes from Awesome Lists.
- https://github.com/JustinGOSSES/nasa_contractor_jobs_information 

---------------------------------
## Existing Longterm Side Projects:
### Geoscience Related Projects
#### Continued improvements to my existing geoscience projects:
1. Wellio
    - Make improvements that remove issues
2. Wellioviz
    - Make improvements that remove issues
 
#### Contribute to existing geoscience community projects:
1. Maintainer of Awesome-open-geoscience: [[https://github.com/JustinGOSSES/awesome-open-geoscience](https://github.com/softwareunderground/awesome-open-geoscience)](https://github.com/softwareunderground/awesome-open-geoscience)
2. Welly:
    - Still need to get to contributing pull requests that make it easier to exchange json between Welly and wellio

### Projects outside geoscience
#### Older Side Projects
1. AR Business cards:
    - fix when dependencies cause it to break
2. 404 page: 
    - done unless browser standards or street view syntax break it again
3. Yi Yun's business site: https://yiyunlininteriors.com/
    - Do adjustments as needed

---------------------------------
## Work In Progress

#### Generative Art 
- Generative objects using "how to draw" or "architecture of " references as inspiration. 
  - Suspect this is very hard approach???
  - Reference for leaves from paleobotanists https://twitter.com/JustinGinHou/status/1393271835442262018?s=19
  - Reference for how to draw bivalves: https://twitter.com/franzanth/status/1390613234382610432?s=19
  - Reference 1980s PDF on algorithmic beauty of plants: https://twitter.com/artnome/status/1396076937626497028?s=19
- Continue:
  - 1. SVG-based on Observable https://observablehq.com/@justingosses/svg-rectangles?collection=@justingosses/generative-ar
    2. 2. SVG-based on Observable https://observablehq.com/@justingosses/generative-curves?collection=@justingosses/generative-art
    3. SVG-based on Observable https://observablehq.com/@justingosses/messing-around-with-a-fork-2342?collection=@justingosses/generative-art

#### Water Relatd
1. Started markdown file with ideas for page that brings together all the sources I check for sea kayaking, whitewater paddling, flat water paddle boarding, and surfing. <a href="https://github.com/JustinGOSSES/sideproject_planning/blob/master/water_activities_dashboard_houston.md">https://github.com/JustinGOSSES/sideproject_planning/blob/master/water_activities_dashboard_houston.md</a>
    - And built <a href="https://github.com/JustinGOSSES/water_check_houston">little page with collection of iframes & visualizations</a> of frequently checked inforrmation sources before paddling.
2. Observable notebook that uses USGS water guage API and personal experiences regarding when water is too high or fast for certain trips and plots the historical periods when trips were or weren't possible on a time series chart. [https://observablehq.com/@justingosses/when-could-you-paddle-buffalo-bayou](https://observablehq.com/@justingosses/when-could-you-paddle-buffalo-bayou

#### "AsBigAs" API
- A tiny javascript library that returns comparisons for length, height, area, volume, and weight based on data in JSONs or CSVs. For example, "The interior of the van has the same volume as 1523 average pineapples." draft in private repo https://github.com/JustinGOSSES/AsBigAs/blob/main/README.md

#### Visual Awesome
Projects Around Community, Connections, & Dependencies:

- <b>"VisualAwesome"</b> SWUNG adaption on Lawrence Livermore National Labs software catalog project with emphasis on understanding engagement band ties across open source geoscience software landscape.
- SWUNG hackathon lightning talk(s) slides
  - Done
- Created easily reusable template repository to decrease the time it takes to adapt the project to other sources from days to dozens of minutes waiting for a script to run after changing several lines in a configuration file: https://github.com/JustinGOSSES/awsome-list-visual-explorer-template
  - Need to improve documentation, fix a few minor bugs, and expand number of visualizations to better answer common questions.
  
#### Maps that speak theme
- **Geology Roadtrip Assistant** Proof of concept in Observable that can be opened with Siri and tells you some key facts about the geologic unit at your present location. The idea is this would be helpful for roadtrips where you didn't have a "Roadside Geology of ___ " book or a passenger willing to check the mile markers and find the right page again and again.
  - Work In Progress Live Notebook: https://observablehq.com/@justingosses/stratigraphy-speech
- **LAGDAL** = Large-language-model Assisted Geology Descriptions of Arbitrary Locations. Demo website for text descriptions of geologic outcrops at arbitrary locations around the world with streetview, geographic map, and geologic map in synchronous movement: [https://github.com/JustinGOSSES/LAGDAL](https://github.com/JustinGOSSES/LAGDAL)
- **Spoken-Floodplain**: Website that verbally tells users when they enter or leave a floodplain in Harris County (Houston) Texas.

--------------------------
## Planning stages only
#### Geoscience
1. Potential future NLP & Geoscience project building on experience with geovec-playground repo???
    - idea
2. Interactive map & pictures of roadcut imagery from google streetview: Reduce time to find useful rock outcrops by training machine learning model to detect road cuts or outcrops that expose bedrock and then place on map with local & regionally based outcrop quality score. 

#### Blog posts & keep personal website updated
?

#### Geospatial
1. Planetary & geospatial notes for later projects : https://github.com/JustinGOSSES/planetary_geospatial_notes/blob/master/README.md
2. Houston (or any scale) kayaking analysis from geospatial data: https://github.com/JustinGOSSES/kayaking_geospatial_project
3. Kayak mapping project is visualization of NLP results of all houston canoe cloud trip reports: https://thcc.clubexpress.com/content.aspx?page_id=22&club_id=496051&module_id=164295

### Geology of Buffalo Bayou 
- Call for interested parties: https://www.hgs.org/buffalo-bayou-geology-project-you-can-help
- NOTES:
    - Reuse of https://github.com/JustinGOSSES/LAGDAL ?
    - Use lidary created DEM from:
      - USGS: https://apps.nationalmap.gov/lidar-explorer/#/
      - preview: https://apps.nationalmap.gov/3depdem/
      - useful static page for checking out local tiff files: https://app.geotiff.io/load
      - useful static apge for checking out COG (cloud optimized geotiff) files: https://geotiffjs.github.io/cog-explorer/#long=168.460&lat=-17.553&zoom=17&scene=&bands=&pipeline=
      - Open Topography: https://opentopography.org/news/api-access-usgs-3dep-rasters-now-available
      - Might be easier if just interested in one area to use this https://github.com/OpenTopography/RiverREM to get tif and use geotiff.js to visualize?
    - Use USGS well logs?
      - (needs fixing again) https://observablehq.com/@justingosses/hello-wellioviz-swap-out-log-no-other-changes-required-now-a?collection=@justingosses/geology
      - bore holes from USGS https://webapps.usgs.gov/nibiMap/index.html
        - Exampel LAS address from that site: https://txdata.usgs.gov/GeoLogArchiver/odata/Logs(5767)/LogFile?Download=true
        - Need to change '.' to '_' for https://justingosses.github.io/wellioviz/demo.html to load the resulting files successfully.
    - Potential modified LAGDAL website for buffalo bayou specific view:
        -  Google streetview imagery
        -  Standard geographic map
        -  clickable visualizatio of borehores
        -  Digital elevation model view
        -  Some way to put depth of borehole onto map, so users can see where something like a gamma ray spike might or might not appear in the bayou outcrop some distance away if continuous horizontally.
        -  Some way to add pictures & notes?

