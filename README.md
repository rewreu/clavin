This docker image uses clavin for geo name tagging, to use it, simply run:
```
docker run -dit -p 9090:9090 eliotjordan/docker-clavin
```

after the docker container starts, create a plain file text.txt with text in it,
then run the following for test:
```
curl -s --data @text.txt --header "Content-Type: text/plain" http://localhost:9090/api/v0/geotag
```
