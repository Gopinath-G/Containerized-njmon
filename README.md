# Containerized-njmon
Deploying njmon in docker containers
Purpose:

Deploy Nigel’s njmon monitoring tool in docker containers
Procedure:

 Pull influxdb and Grafana images from docker repository (grgopinath/containerized_njmon) and deploy it as individual containers or services in swarm cluster

Ports:

 Below ports are exposed in respective container images and it must be published.
Influxdbv1:

   -    Ports 8086 and 8181
Grafanav1

   -    Ports 3000
 
 Depoy using the docker file
 
 example:
 docker stack deploy -c docker-compose.yml njmon
