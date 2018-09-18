# multi-docker
try multi-docker build to dockerhub and deploy to aws

build fib multi-container app image
```
  > cd client
  > docker build -f Dockerfile.dev -t smalltides/fib-client .
  > docker run smalltides/fib-client
  > cd ..
  > cd server
  > docker build -f Dockerfile.dev -t smalltides/fib-server .
  > docker run smalltides/fib-server
  > cd ..
  > cd worker
  > docker build -f Dockerfile.dev -t smalltides/fib-worker .
  > docker run smalltides/fib-worker
```
run fib multi-container app
```
  > docker-compose up
```
