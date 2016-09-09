This module loads geospatial data from MapCruzin (www.mapcruzin.com) into OrientDB.


How to install (requires Node.js):
```
npm init
npm install orientjs
npm install fast-csv
npm install
```

How to start:

1. Install OrientDB (latest stable - http://www.oriendb.com) 
2. Install OrientDB Geospatial module (see http://orientdb.com/docs/2.2/Spatial-Index.html)
3. Start OrientDB server and create a new DB 
4. Open the DB from Studio and execute the following statements:
   ```
   CREATE CLASS POI
   CREATE PROPERTY POI.location EMBEDDED OPoint
   ```
5. From a shell, in the root project directory
   ```
   > node csvimport.js POI data/poland-poi.csv 
   ```
   
For help and parameter list, just type the following:

   ```
   > node csvimport.js
   ```

