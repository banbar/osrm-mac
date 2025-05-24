docker run --rm -v "${PWD}:/data" stefda/osmium-tool     osmium cat /data/map.osm -o /data/map.pbf --overwrite -f pbf
