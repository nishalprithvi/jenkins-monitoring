# jenkins-monitoring

it is dcoker compose yaml file, here we run the entire ecosystem on docker compose or on docker instances.
some points to keep in mind before executing this docker-compose file, you need to first run the docker compose up that will create the docker volume 
directories in your system then  you should set 777 permissions for the the volume directories again restart the docker compose.
after setting up the volume directory you also need to setup prometheus.yml file configuration of the prometheus you can use the sample prometheus config file,
need to update about it in the docker compose file.

post this the docker instances would up you need to setup all the plugins in jenkins and dahboard in grafana, remember to use your machine ip address for mapping 
the urls in prometheus.yml, in jenkins for influxdb.

For more refferal and setting up influx db, grafana & jenkins look -https://youtu.be/AHSHksfg1BE
