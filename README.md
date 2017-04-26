# meshblu-docker-compose
Run the meshblu stack using docker compose

## Prerequisites

* [Docker 1.13 or higher](https://docs.docker.com/engine/installation/)

## Run

```shell
# replace meshblu with your own stack name if desired
docker stack deploy -c ./docker-compose.yml meshblu
```

## Customize

If you intend to use this for production use, you should modify the environment variables in `meshblu-core-dispatcher.env` and `meshblu-core-protocol-adapter.env`. Specifically, you'll want to change the variables: TOKEN, PRIVATE_KEY_BASE64, and PUBLIC_KEY_BASE64 in `meshblu-core-dispatcher.env`
