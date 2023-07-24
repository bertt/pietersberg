# pietersberg

Demo: Create Terrain Tiles from AHN4 Laseraltimetry data

Demo: https://bertt.github.io/pietersberg/index.html

![image](https://github.com/bertt/pietersberg/assets/538812/768fd32e-33b8-4e97-8e88-cec1715c00e5)

To run:

```
$ wget https://ns_hwh.fundaments.nl/hwh-ahn/ahn4/01_LAZ/C_69AZ2.LAZ 
6.1GB
$ pdal pipeline pipeline.json
$ docker run -v $(pwd):/data -it geodan/terrainwarp
$ docker run -v $(pwd):/data -it geodan/terraintiler
$ wget https://raw.githubusercontent.com/Geodan/terrain/main/samples/maastricht/index.html
$ python -m http.server 8000
```
