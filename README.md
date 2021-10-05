# How to run product page

## Prerequisite

* Python 3.8

```bash
pip install -r requirements.txt
python productpage.py 9080
```
# itkmitl-bookinfo-productpage
```bash
# Build Docker Image for productpage service
docker build -t webpage .

# Run Python
docker run -d --name productpage -p 8083:8083 --link details:details --link ratings:ratings --link reviews:reviews -e 'REVIEWS_HOSTNAME=http://reviews:9080' -e 'RATINGS_HOSTNAME=http://ratings:8080' -e 'DETAILS_HOSTNAME=http://details:8081' productpage

* Test with Port 8083
```

## How to run with Docker Compose

```bash
docker-compose up
```
