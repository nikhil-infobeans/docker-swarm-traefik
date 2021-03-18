# docker-swarm-traefik

Swarm Setup
```
$ docker swarm init
$ docker network create --driver=overlay traefik-public
$ docker stack deploy -c stack.yml demoapp
```
Get the IP address 
Add host entry 
```
IP_ADDRESS   demoapp.local
```

Open the browser and hit the below URL

| http://demoapp.local:8030/

Exit from the docker Swarm mode - 
```
docker swarm leave -f
```
