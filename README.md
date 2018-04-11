

# Instructions to build docker from scratch
```
mkdir node-web-app
cd node-web-app/

wget https://gist.githubusercontent.com/pafmon/e27e7b9ad5b1dcbc9a3c34b781e2746c/raw/33998dc4d26080f3cfa928f7f758e1bc85ab20a4/.dockerignore
wget https://gist.githubusercontent.com/pafmon/e27e7b9ad5b1dcbc9a3c34b781e2746c/raw/33998dc4d26080f3cfa928f7f758e1bc85ab20a4/Dockerfile
wget https://gist.githubusercontent.com/pafmon/e27e7b9ad5b1dcbc9a3c34b781e2746c/raw/33998dc4d26080f3cfa928f7f758e1bc85ab20a4/package.jso
wget https://gist.githubusercontent.com/pafmon/e27e7b9ad5b1dcbc9a3c34b781e2746c/raw/33998dc4d26080f3cfa928f7f758e1bc85ab20a4/package.json
wget https://gist.githubusercontent.com/pafmon/e27e7b9ad5b1dcbc9a3c34b781e2746c/raw/33998dc4d26080f3cfa928f7f758e1bc85ab20a4/server.js

docker build -t pafmon/node-web-app .
docker images
docker run -p 49160:8080 -d pafmon/node-web-app
docker ps
docker logs 1a

docker login
docker push pafmon/node-web-app
```
