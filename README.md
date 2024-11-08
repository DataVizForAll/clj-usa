# clj-usa
census tract geodata and pre-post-2023 crosswalk for Center for Leadership &amp; Justice, Urban Suburban Affordables community land trust

## Five towns where most CLJ USA homes are located
Bloomfield
East Hartford
Hartford
West Hartford
Windsor

## GeoJSON files
- clj-usa-boundary.geojson = outline of five-town boundary
- clj-usa-towns.geojson = outlines of each of the five towns
- clj-usa-tracts-2023.geojson = census tracts located in the five towns

## Crosswalk CSV file
- crosswalk.csv
- also available in [this Google Sheet](https://docs.google.com/spreadsheets/d/1FuPltpxKEWunwLLlfEUgAt8yB7E_1AY_Qt2ci14mzaU/edit?gid=1021595254#gid=1021595254) 

In 2023, the US Census Bureau shifted its data coding away from 8 CT counties (which were technically abolished in 1960 by CT legislature) to 9 CT planning regions (aka county-level equivalents). [Read more by CTData.org](https://www.ctdata.org/blog/geographic-resources-for-connecticuts-new-county-equivalent-geography)

While this shift did not alter the census tracts, it did change the longer FIPS or GEOID codes for each tract, because the middle characters refers to the county-level area.

This "crosswalk" helps to connect old and new census tract longer code numbers, and it's especially designed for Datawrapper mapping with our custom GeoJSON.

| Column Header  | Example     | Definition                                                                                                                         |
|----------------|-------------|------------------------------------------------------------------------------------------------------------------------------------|
| ShortTractText | 503102      | Short census tract, same before and after 2023, in text format to match custom GeoJSON file above                                  |
| GEOID2023Text  | 09110503102 | Longer census tract code after 2023: 09 = CT, 110 = Capitol Planning Region (new county-level equivalent)                          |
| GEOID2022Text  | 09003503102 | Longer census tract code before 2023: 09 = CT, 003 = Hartford County (which US Census stopped using after 2022)                    |
| ShortTractNum  | 5031.02     | Short census tract, in numerical format to display decimals for tracts that were split prior to 2020 (such as 5031.01 and 5031.02) |

## Credit
Created by Jack Dougherty, Trinity College in November 2024 for <https://DataVizForAll.org>
