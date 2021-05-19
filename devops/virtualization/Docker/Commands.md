1. Get a new container up and running, on specified port:
`docker container run -p 80:80 --name {name} -d {image}`

2. Inspect running container:
`docker container inspect {name}`

3. bash into a running container:
`docker container exec -it {name} bash`

4. gets stats of a running container:
`docker stats {name}`

5. **create**&**inspect** new network:
`docker network create|inspect {name}`

6. Connect new container to existing network:
`docker container run -d --name {name} --network {network} {image:'nginx'}`

7. Ping container on same network
`docker container exec -it {container_1} ping {container_2}`