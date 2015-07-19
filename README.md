# mkgmap-style-sheets
This project aims to improve the vector maps for Garmin GPS created with the mkgmap compiler from http://OpenStreetMap.org data for the world routable maps at http://garmin.openstreetmap.nl and the routable bicycle map from http://www.openfietsmap.nl

Please report issues at the OSM forum: http://forum.openstreetmap.org/viewtopic.php?id=13257
or http://forum.openstreetmap.org/viewtopic.php?id=2625

# mkgmap parameters for the generic new style

Example of the parameters in the mkgmap.args file.
For more details http://www.mkgmap.org.uk/doc/index.html

name-tag-list: name:en,int_name,name,name:nl,name:fr,name:de,place_name
generate-sea: land-tag=natural=background
precomp-sea:  sea_latest.zip
bounds:  bounds_latest.zip
location-autofill: is_in,nearest
housenumbers
tdbfile
latin1
code-page: 1252
#code-page: 65001
#lower-case
show-profiles: 1
#ignore-maxspeeds
#remove-short-arcs
min-size-polygon: 4
polygon-size-limits=17:2, 15:0
#reduce-point-density=3
#reduce-point-density-polygon=3
merge-lines
add-pois-to-areas
add-pois-to-lines
link-pois-to-ways
#ignore-turn-restrictions
make-opposite-cycleways
process-destination
process-exits
preserve-element-order
keep-going
net
route 
index
nsis
gmapsupp
copyright-message: Map data © Openstreetmap.org

# mkgmap parameters for Openfietsmap

generate-sea: land-tag=natural=background
precomp-sea:  sea_latest.zip
bounds:  bounds_latest.zip
location-autofill: is_in,nearest
housenumbers
name-tag-list: name,name:nl,name:fr,name:de,int_name,place_name
tdbfile
latin1
code-page: 1252
show-profiles: 1
min-size-polygon: 4
polygon-size-limits=17:2, 15:0
merge-lines
add-pois-to-areas
add-pois-to-lines
link-pois-to-ways
preserve-element-order
keep-going
net
route
index
copyright-message: Map data © openstreetmap.org, Map layout © openfietsmap.nl, SRTM Data © U.S. Geological Survey
#remove-ovm-work-files: true
#ignore-turn-restrictions
#ignore-maxspeeds
#remove-short-arcs

More info on http://www.openfietsmap.nl/procedure