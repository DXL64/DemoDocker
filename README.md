# DemoDocker

Run Docker
```bash
docker build -t <image_name> .
docker run -dp <port>:6040 --name <container_name> <image_name>
```
Example
```bash
docker build -t demo .
docker run -dp 3000:6040 --name demo_c demo
```

Run Docker Compose 

Edit container and image name in docker-compose.yaml
```bash
docker compose up
```
