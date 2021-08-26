# Build your image
docker build . -t <your username>/node-web-app

# Check docker images
docker images

# Run docker image
docker run -p 49160:8081 -d <your username>/node-web-app

# Get container ID
$ docker ps

# Print app output
$ docker logs <container id>

# Example
Running on http://localhost:8080

# Enter the container
$ docker exec -it <container id> /bin/bash

# Call App or Testing access
$ curl -i localhost:49160

HTTP/1.1 200 OK
X-Powered-By: Express
Content-Type: text/html; charset=utf-8
Content-Length: 12
ETag: W/"c-M6tWOb/Y57lesdjQuHeB1P/qTV0"
Date: Mon, 13 Nov 2017 20:53:59 GMT
Connection: keep-alive

Hello world
