# Alpine Docker Image with curl, jq, bash

### Use Cases:
* Quick `curl` during multi step build config
* `curl` api to verify access control and proceed further steps.

### Usage
Pull docker image `docker pull stfnralpine-curl-jq`

### Example
**curl**
```
docker run stfnr/alpine-curl-jq curl https://www.google.com
```
**curl, jq**
```
docker run stfnr/alpine-curl-jq curl -s https://api.github.com/repos/github/hub/forks | jq .[].id
```

### Reference

https://github.com/dwdraju/alpine-curl-jq
