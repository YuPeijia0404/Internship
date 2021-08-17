# Docker
### Useful commands
* Delete all images
    * `docker rmi -f $(docker images -a -q)`
* Delete all containers (include those in use)
    * `docker rm -vf $(docker ps -a -q)`