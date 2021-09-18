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
docker run -d --name webpage -p 8083:8083 webpage

* Test with Port 8083
```