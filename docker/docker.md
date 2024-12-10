# Docker

## Docker Installation
### Windows
[https://docs.docker.com/desktop/setup/install/windows-install/](https://docs.docker.com/desktop/setup/install/windows-install/)

### MacOS
[https://docs.docker.com/desktop/setup/install/mac-install/](https://docs.docker.com/desktop/setup/install/mac-install/)

### Linux
[https://docs.docker.com/desktop/setup/install/linux/](https://docs.docker.com/desktop/setup/install/linux/)


## Useful commands
List all running containers
```sh
docker ps
```
Use `-a` option for all containers
```sh
docker ps -a
```

Follow logs
```sh
docker logs -f {container_id_name}
```

Stop container
```sh
docker stop {container_id_name}
```

Shell into container
```sh
docker exec -it {container_id_name} sh
```
