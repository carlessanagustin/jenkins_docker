# Jenkins container in Docker Compose

## Requirements

* Docker Engine
* Docker Compose

## Commands

* Run: `docker-compose up -d`
* Get initial password

```shell
docker exec -i <container_id> \
    cat /var/jenkins_home/secrets/initialAdminPassword
```
