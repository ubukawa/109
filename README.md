# 109
dowloading pbf and make PMtiles (This is just for test). The data should not be used for other purpose.

# source
https://pro-ags2.dfs.un.org/arcgis/rest/services/Hosted/Clearmap_Webplain/VectorTileServer/tile/{z}/{y}/{x}.pbf

## Terms of use (from the original data)
* https://geoservices.un.org/Html5Viewer/index.html?viewer=clearmap
* https://geoportal.un.org/arcgis/home/item.html?id=541557fd0d4d42efb24449be614e6887


# Usage
```
gid clone https://github.com/ubukawa/109
cd 109
docker run -it --rm -v ${PWD}:/data unvt/nanban
cd /data
./mkdir.sh
./download.sh  
./delete-null.sh
```