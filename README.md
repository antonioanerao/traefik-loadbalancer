# Traefik com Load Balancer

Este projeto implementa um ambiente Docker usando o Traefik como um load balancer que configura sessões persistentes com cookies sticky para garantir que usuários retornem ao mesmo container. 

### Crie uma nova subrede (opcional)

Antes de subir a stack com _docker compose up -d_, crie uma subrede chamada _proxy_<br>
Adapte o docker-compose.yml se não criar a nova subrede

```bash
docker network create proxy
```

### Suba a stack

```bash
docker compose up -d
```

### Painel Traefik

```
http://localhost:8080
```

### URL dos webserver nginx

```
http://webserver.docker.localhost
```
