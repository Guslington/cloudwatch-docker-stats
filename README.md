# Cloudwatch Docker Stats
-------------------------

## Run
```
docker run -dit --name cw \
  -e "CONTAINERS=container1,container2" \
  -e ENVIRONMENT=develop \
  -e CLOUDWATCH_REGION=ap-southeast-2 \
  -v /var/run/docker.sock:/var/run/docker.sock \
  cloudwatch-docker-stats
```
