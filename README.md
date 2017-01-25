# sitka-buildings
![sitka-buildings][image]
# Update 2017-01-09

The buildings import is complete and this repository is no longer maintained. OpenStreetMap is now the most current source for Sitka's buildings.

To get the latest buildings with elevation and height data use the OpenStreetMap editor JOSM. Select the Sitka area and download. Save the .osm file and use osm2pgsql with the buildings.style included in this repository.

`osm2pgsql -cGs -d osm -S /sitka-buildings/buildings.style ~/Downloads/your_file.osm.`

This style filters out excess OSM fields that aren't necessary for buildings but other ways will still be present. Use a '"building" is NOT NULL' query to filter out other ways.

--------

Process for importing Sitka area buildings and addresses to OpenStreetMap with height information

Building footprints were drawn from 2012 imagery publicly available [here](http://dggs.alaska.gov/file_transfer/CityOfSitka_data/Imagery%20Sid/Sitka_2012.sid)

Heights were extracted using the footprint polygon's centroids and a point sampling tool to find the difference between the highest hit and the bare earth DEMs. These DEMs were created by FEMA and are in the public domain and hosted by DGGS [here] (http://dggs.alaska.gov/file_transfer/CityOfSitka_data/LiDAR%20Originals/)

[image]:https://c1.staticflickr.com/1/726/32425895635_08ba8b2e2b_z.jpg "Buildings colored by height"
