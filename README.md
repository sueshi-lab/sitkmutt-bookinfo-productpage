# Bookinfo Productpage Service

Productpage service has been developed on Python

## License

MIT License

## How to run with Docker

```bash
# Build Docker Image for productpage service
docker build -t productpage .

# Run productpage service on port 8083
docker run -d --name productpage -p 8083:8083 --link details:details --link ratings:ratings --link reviews:reviews -e DETAILS_HOSTNAME=http://details:8081 -e RATINGS_HOSTNAME=http://ratings:8080 -e REVIEWS_HOSTNAME=http://reviews:9080 productpage
```

## How to run with Docker Compose

```bash
docker-compose up
```

## Website

[Opsta (Thailand) Co., Ltd.](https://www.opsta.co.th)
