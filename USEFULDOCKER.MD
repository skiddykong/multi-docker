docker system prune -a -f

docker volume prune

docker volume rm $(docker volume ls -qf dangling=true)
