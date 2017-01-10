# sitka-buildings

# Update 2017-01-09

The buildings import is complete and this repository will no longer be maintained. The buildings on OpenStreetMap are now the most current source for Sitka's buildings.

--------

Process for importing Sitka area buildings and addresses to OpenStreetMap with height information

Building footprints were drawn from 2012 imagery publicly available [here](http://dggs.alaska.gov/file_transfer/CityOfSitka_data/Imagery%20Sid/Sitka_2012.sid)

Heights were extracted using the footprint polygon's centroids and a point sampling tool to find the difference between the highest hit and the bare earth DEMs. These DEMs were created by FEMA and are in the public domain and hosted by DGGS [here] (http://dggs.alaska.gov/file_transfer/CityOfSitka_data/LiDAR%20Originals/)
