A secure CSV file uploading web app using open source software & libraries.

# Usage
```
docker run -d --name av mkodockx/docker-clamav
```
```
docker run -d --link av:clamavd -p 8090:8090 --name secure-csv-uploader immontilla/secure-file-uploader
```

**Access the web app**
```
http://localhost:8090/
```

**Gain access to the console**
```
docker exec -it secure-csv-uploader sh
```

**List the docker volumes**
```
docker volume ls
```

**See information about the volume *csv-files***
```
docker volume inspect csv-files
```

**List the uploaded files**
```
sudo ls -l /var/lib/docker/volumes/csv-files/_data
```

**See the secure-csv-uploader log**
```
docker logs secure-csv-uploader
```
