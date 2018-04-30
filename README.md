# Jersey City 2018 Revaluation

This repo: [https://github.com/code4jc/jcreval/](https://github.com/code4jc/jcreval/blob/master/.gitignore)

## Data and Information Sources


- Appraisal Systems (vendor performing revaluation for City of Jersey City)
  - [Main landing page](http://www.asinj.com/revaluation.asp?p=current&id=359) for Jersey City 2018 revaluation.
  - Proposed Residential Assessments [(xls)](http://www.asinj.com/revaluation/docs/assessmentlists/359/Proposed%20Assessments%20as%20of%20April%2018th.xlsx). Last update April 18th.

  
- City of Jersey City
    - Official [reval page](http://www.cityofjerseycity.com/CityHall/taxes/reval/) on the city's website.


- NJGIN (New Jersey Geographic Information Network)
  - Hudson country [parcel maps](https://njgin.state.nj.us/NJ_NJGINExplorer/IW.jsp?DLayer=Parcels%20by%20County/Muni
  
## Preparation & Analysis Methods

1. PAMS PIN column added using method specified in [http://njwebmap.state.nj.us/NJGeoWeb/Webpages/Info/Help/PAMSPIN.html](http://njwebmap.state.nj.us/NJGeoWeb/Webpages/Info/Help/PAMSPIN.html). This is a unique property identifier used to join the reval data with the parcel basemap.
2. TO DO
  -fix PAMS_PIN concatentation for parcels that have a QCODE (mostly multi-unit parcels like condos) 
  -strip $ and , from all the money fields (e.g. convert strings to numbers)
3. TBD. Much more to come.

## Methods

1. Mostly using QGIS for visualization.

## Gallery

## Related Work

- Dan Goldin has a great notebook [here](https://github.com/dangoldin/jersey-city-tax-assessment) that plots the April 18 release on a Google Maps basemap. 