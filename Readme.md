docker run --rm -v "${PWD}:/data" stefda/osmium-tool     osmium cat /data/map.osm -o /data/map.pbf --overwrite -f pbf

docker run --rm -t -v "/Users/banbar/Desktop/web_atolye/data:/data" osrm/osrm-backend     osrm-extract -p /opt/foot.lua /data/foot/map.pbf
docker run --rm -t -v "/Users/banbar/Desktop/web_atolye/data:/data" osrm/osrm-backend     osrm-extract -p /opt/car.lua /data/car/map.pbf
docker run --rm -t -v "/Users/banbar/Desktop/web_atolye/data:/data" osrm/osrm-backend     osrm-extract -p /opt/bicycle.lua /data/bicycle/map.pbf
