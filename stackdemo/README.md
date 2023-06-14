# Grupo:
- Alessandra Avelino
- Hacjesse Barbosa


# Comandos 
docker system info

docker swarm init

docker node ls

docker service create --name registry --publish published=5000,target=5000 registry:2

docker service ls

curl http://localhost:5000/v2/

docker-compose up -d

docker-compose ps

docker-compose down --volumes

docker run -d -p 5000:5000 --restart=always --name registry registry:2

docker-compose push

docker stack deploy --compose-file docker-compose.yml stackdemo

docker stack services stackdemo

# Quando estiver tudo certo, os "workers", devem acessar:
docker swarm join --token SWMTKN-1-0skuoeo43iony24cg3dex89j32i0vy7eltcju36kwl3o7dsmpv-8rvibkkatc7d8mbj0vvoj07se 10.10.132.22:2377
