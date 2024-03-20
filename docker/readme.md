 # Run
 docker compose -f docker-compose.yml up -d

 ## Check the container
 docker ps
 
 ## Add nginx
 docker tag nginx localhost:5000/nginx:version1
 
 ## Check network
 docker network ls

 ## Inspect container ID
 docker inspect container_ID

 ## Expose le backend
 docker compose -f docker-compose.yml down

 ## Push notre image nginx
 docker push localhost:5000/nginx:version1

 ## Kill container
 docker compose -f docker-compose.yml down

