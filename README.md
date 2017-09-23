# redash-with-traefik
A :whale: docker based Redash setup with Traefik

## How to deploy?
### 1. Change variables
Once the repo is cloned, open `docker-compose.yml` and replace all the variables with
```sh
# <-- Change this
```
the above comment.

 :point_up: Do the same with `traefik.toml` as well.
 
### 2. Create acme.json
```sh
$ touch acme.json
```

### 3. Start the containers
```sh
$ docker-compose up -d
```
This will start all the containers required to run redash and traefik.

### 4. Create db
```sh
$ docker-compose run --rm server create_db
```

Now go to the url where you deployed it and set it up!


## License

MIT
