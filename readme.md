### Documentation

*usage: "Rake dataset title="title" link="http://dataurl.com"*

#### Usage

name | meaning | format | example |
---- | ---- | ---- | ---- |
title | title | text | title="2013 Congressional Districts Shapefile" |
tags | tags | array | tags="2013, congress, redistricting" |
pub | publication date | month/year or 00/year |  
desc | description | text | desc="This shapefile shows the revised Congressional districts following the 2010 Census." |
shp | shapefile | url/filepath | shp="../data/2013_cong_districts.shp" |
csv | comma separated value dataset | url/filepath | csv="http://docs.google.com" |
sql | associated sql statement |  url/filepath |  sql="../metadata/0001-01-01-sql-statement.md" |
map | MapBox map API | username.mapname | map="herwig.map-wgt" |
link | source link | url/filepath to content origin/attribution | link="http://dailykos.com" |
source | source name | text | source="Cicero API by Azavea" |
pdf | pdf file associated with dataset | url/filepath | pdf="http://census.gov/documentation.pdf" |
parents | is the dataset associated with/a derivative of any other sets? | url/filepath | parents="../data/0001-01-01-parent-data.md" |
category | stage in data processing | [raw, extraction, clean] | category="raw" |

#### Example

```sh
rake dataset title="2013 Congressional Districts Shapefile" \
 tags="2013, congress, redistricting" \
 desc="This shapefile shows the revised Congressional districts following the 2010 Census." \
 shp="../data/2013_cong_districts.shp"  \
 csv="http://docs.google.com" \
 sql="../metadata/0001-01-01-sql-statement.md" \
 map="herwig.map-wgt" \
 link="http://dailykos.com" \
 source="Cicero API by Azavea" \
 pdf="http://census.gov/documentation.pdf" \
 parents="../data/0001-01-01-parent-data.md" \
 category="raw" \

```


