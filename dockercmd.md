<!-- Build docker image -->

docker build -t fileName .

<!-- insure the expose the localhost for next -->

docker run -p 3000:3000 crm-docker

<!-- if somethings change in the file or modified -->
<!-- but too much complex and writing -->

docker run -p 3000:3000 -v "$(pwd):/app" -v /app/node_modules crm-docker

<!-- if you want to see all container -->

docker ps -a

<!-- if you want to stop specific container -->

docker stop containerName

<!-- if you want to stop all container running also delete container-->

docker container prune

<!-- if you want to delete or force stop delete while running -->

docker rm containerName --force

<!-- if you want to upload image into docker hub -->

docker tag filename username/filename
docker push username/filename

<!-- if you want not manually but automatic like npm init -->

docker init
docker compose up

<!-- after editing the compose.yaml in order to keep updated -->

docker compose watch
