Running Docker

// create docker image called mern-stack-web
 
 docker build -t mern-stack-web
 docker run -p 5000:5000 --rm -e MONGO_USER=Pirlobo -e MONGO_PASS=<password> mern-stack-web

// Play with docker hub 

open cmd 
docker login 
docker tag mern-stack-web:latest pirlobo/mern-stack-web
docker push pirlobo/mern-stack-web

// Visit Docker Hub Page 

docker pull pirlobo/mern-stack-web
docker run -p 5000:5000 --rm -e MONGO_USER=Pirlobo -e MONGO_PASS=<password> mern-stack-web

Click "Open" with port 5000 to run the applciation
