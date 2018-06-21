# Rails Passenger Docker

Base repository when building rails applications using passenger-docker.

## Command

### Build

```
$ docker build -t rails-image .
```

### Run

```
$ docker run \
  -p 3000:80 \
  -e DB_HOST=xxxxx \
  -e DB_USER=xxxxx \
  -e DB_PASSWORD=xxxxx \
  -e DB_DATABASE=xxxxx \
　　　　-e RAILS_MASTER_KEY=xxxxx \
　　　　-e RAILS_LOG_TO_STDOUT=ON \
  rails-image
```
