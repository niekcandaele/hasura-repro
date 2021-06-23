Reproduction case for https://github.com/hasura/graphql-engine/issues/7089

```sh
docker-compose up -d

# verify the server is up and running
curl http://127.0.0.1:8080/v1/version

docker-compose up -d && docker-compose logs -f repro
# Might need to ctrl+c and redo this last command to make sure repro container fires after Hasura container
```