# sitka-buildings
Process for importing Sitka area buildings and addresses to OpenStreetMap with height information

Building footprints were drawn from 2012 imagery publicly available [here](http://dggs.alaska.gov/file_transfer/CityOfSitka_data/Imagery%20Sid/)

Heights were extracted using the footprint polygon's centroids and a point sampling tool to find the difference between the highest hit and the bare earth DEMs that are publicly available [here](http://dggs.alaska.gov/file_transfer/CityOfSitka_data/LiDAR%20Originals/)
