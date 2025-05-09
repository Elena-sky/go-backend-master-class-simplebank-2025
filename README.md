# Backend Master Class [Golang + Postgres + Kubernetes + gRPC]

Link to the course https://www.udemy.com/course/backend-master-class-golang-postgresql-kubernetes/

## Setup local development

### Install tools

- [Docker desktop](https://www.docker.com/products/docker-desktop)
- [TablePlus](https://tableplus.com/)
- [Golang](https://golang.org/)
- [Homebrew](https://brew.sh/)
- [Migrate](https://github.com/golang-migrate/migrate/tree/master/cmd/migrate)

    ```bash
    brew install golang-migrate
    ```

- [Sqlc](https://github.com/kyleconroy/sqlc#installation)

    ```bash
    brew install golang-migrate
    ```

### Setup infrastructure

- Start postgres container:

    ```bash
    make postgres
    ```

- Create simple_bank database:

    ```bash
    make createdb
    ```

- Run db migration:

    ```bash
    make migrateup
    ```



Useful links
- [DB diagram website](https://dbdiagram.io/home)
- [Go Playground](https://go.dev/tour/welcome/1)
- [Sqlc's documentation page](https://docs.sqlc.dev/en/stable/tutorials/getting-started-postgresql.html)


Docker 
- Pull an image `docker pull <immage>:<tag>`
- Start a container `docker run --name <container_name> -e <environment_variable> -d <image>:<tag>`
- Port mapping `docker run --name <container_name> -e <environment_variable> -p <host_ports:container_ports> -d <image>:<tag>`
- Run command in container `docker exec -it <container_name_or_id> <command> [args]`
- View container logs `docker logs <container_name_or_id>`

Running the project
