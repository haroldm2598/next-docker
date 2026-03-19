<!-- Build docker image -->

docker build -t fileName .

<!-- insure the expose the localhost for next -->

docker run -p 3000:3000 crm-docker

<!-- if you want to see all container -->

docker ps -a

<!-- if you want to stop specific container -->

docker stop containerName

<!-- if you want to stop all container running also delete container-->

docker container prune

<!-- if you want to delete or force stop delete while running -->

docker rm containerName --force
