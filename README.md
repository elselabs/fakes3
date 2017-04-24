# Elselabs FakeS3 docker container

Fake AWS S3 server for local development based on [fake-s3](https://github.com/jubos/fake-s3). Runs in docker.

Usage (in docker-compose.yml):
```
  fakes3:
    container_name: fakes3
    image: elselabs/elselabs-fakes3
    ports:
      - "4567:4567"
    volumes:
      - ./tmp:/fakes3/data
   
```
