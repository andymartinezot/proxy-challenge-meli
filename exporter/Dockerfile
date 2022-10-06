FROM nginx/nginx-prometheus-exporter
#CMD ["-nginx.scrape-uri", "http://192.168.0.53:8080/nginx_status"]
CMD ["-nginx.scrape-uri", "http://${DOCKER_GATEWAY_HOST:-host.docker.internal}:8080/nginx_status"]

#On both macOS and Windows it works out of the box now without anything left to do.
#If you are running this stack on Linux you need to have the DOCKER_GATEWAY_HOST environment variable set for the Docker gateway host. Simply put this line into your .bashrc (.bash_profile or .zshrc):
#export DOCKER_GATEWAY_HOST=172.17.0.1

#Dockerfile created by Andy Martinez @andymartinezot in linkedin
