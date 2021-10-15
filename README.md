How to build?

docker build -t polyu20043839d/student_svc .

How to Run?
1. clone the MongoDB repo

git clone https://github.com/cswclui/mongodb-docker

2. run the docker container

cd mongodb-docker
docker-compose up

3. pull the image

docker pull polyu20043839d/student_svc

4. run it as container

docker run --rm --network ass1 -e MONGO_USERNAME=comp3122 -e MONGO_PASSWORD=12345 -e MONGO_SERVER_HOST='mongo' -e MONGO_SERVER_PORT='27017' -p 9990:15000 polyu20043839d/student_svc
