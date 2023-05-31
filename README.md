# DockerLocalhost

Docker Localhost Test Container

## Usage

Change theese parts in docker-compose.yml

```yml
            MYSQL_ROOT_PASSWORD: __MYSQL_ROOT_PASSWORD__
            MYSQL_DATABASE: __MYSQL_DATABASE__
            MYSQL_USER: __MYSQL_USER__
            MYSQL_PASSWORD: __MYSQL_PASSWORD__
```

## Build

```bash
docker build -t docker-localhost .
```

## Run

```bash
docker run -d -p 80:80 docker-localhost
```

## Test

```bash
curl http://localhost:801/
curl http://localhost:802/
curl http://localhost:8080/
```
