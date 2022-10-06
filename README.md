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
curl http://127.0.0.1:8080/nginx_status
```

Check the Nginx metrics in Prometheus metrics format:
```
http://127.0.0.1:9113/metrics
```

Check the Nginx metrics in Prometheus:
```
http://127.0.0.1:9090
```

## Solution diagram
![diagram](https://user-images.githubusercontent.com/77750560/194356318-be7cd5b6-4a12-40e6-b48f-263c4ceb9bce.jpg)

## Notes
* Proxy exclusively created with [Nginx](https://www.nginx.com/)![Uploading diagram.png…]()

* The proxy is configured to accept 50000 requests per second.
* It's possible to filter the requests based on IP addresses (change nginx.conf)
