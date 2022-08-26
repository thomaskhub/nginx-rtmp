# nginx-rtmp
A nginx-rtmp server used for ums develeopment and prodction. 
The docker file was original used from [nginx-rtmp](https://hub.docker.com/r/tiangolo/nginx-rtmp/)
The Dockerfile is pretty much the same, only the nginx configuration has been adapted for ums development and production 
environment. 

# Build the docker image 
```bash 
git clone git@github.com:thomaskhub/nginx-rtmp.git 
cd nginx-rtmp.git 

docker build -t ums-nginx-rtmp .
```

# Start the docker container 
```bash 
docker run -d -p 1935:1935 --name ums-rtmp ums-nginx-rtmp
```

# License
This project is licensed under the terms of the MIT License.


