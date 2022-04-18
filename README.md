# Proxy Challenge MELI

API Proxy developed for the Mercado Libre technical challenge.

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.


### Prerequisites
https://www.docker.com/get-started

#### Development Profile

Run in the command line:
```
docker-compose up -d
```

Test the proxy:
```
curl http://127.0.0.1:8080/categories/MLA5725
```

Check the statistics of the proxy:
```
http://http://127.0.0.1:8080/nginx_status
```

## Solution diagram
