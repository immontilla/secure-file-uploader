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

**Access to the console**
```
docker exec -it secure-csv-uploader sh
```

**List the uploaded files**
```
docker exec -it secure-csv-uploader sh -c "ls -l /tmp/safe"
```

**See the secure-csv-uploader log**
```
docker logs secure-csv-uploader
```
