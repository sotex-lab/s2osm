# s2osm

### Scripts
```bash
docker exec -it map ./populate_data
```
This will download the data for Nigeria, for other countries you can either modify the script or download the data manually here: https://download.geofabrik.de/africa.html.

> [!IMPORTANT]
> Path to the file must be added to the .env file, it's simplest if you put it in /data directory of the repository.

### .env File Contents

```bash
DATABASE=[PATH_TO_PBF] # Example: DATABASE=./data/nigeria.osm.pbf
IMPORT=[import/run] # Either choose import for first time pbf load or run if the data is loaded.
```

> [!IMPORTANT]  
> Import of the data takes a while (about 10 minutes and will exit on completion, do not stop it!

### Running

```bash
docker compose up
```
