# How to dockerize your local wordpress development and prepare for deploying wordpress site to production

1. Install Docker on your local machine
2. Run Docker
3. Create a folder from which you will run docker-compose commands
4. Name the folder whatever you wich eg. example
5. Create **docker-compose.yaml** file
6. Run:

`docker-compose up -d`

7. Open your new WodPress webiste in the browser and finish the installation process

`http://example.test:8000`

## Some useful Docker commands which you may need to know

### Stop all containers if they are running

Check running containers first

`docker ps`

This is an IS of a running container: 74e6ed9e7a2c

`docker container stop --time 30 74e6ed9e7a2c`

Remove the stopped containers

Check all containers (even the stopped ones)

`docker ps -a`

`docker container rm 74e6ed9e7a2c`

Clean all: containers, images, volumes

```
docker container ls -a / docker ps -a
docker container rm <id> -f
docker image ls -a
docker image rm <id> -f
docker volume ls
docker volume rm <id> -f

```
