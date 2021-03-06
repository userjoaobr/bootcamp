# Adonis API application

This is the boilerplate for creating an API server in AdonisJs, it comes pre-configured with.

1. Bodyparser
2. Authentication
3. CORS
4. Lucid ORM
5. Migrations and seeds

## Setup

Use the adonis command to install the blueprint

```bash
adonis new yardstick --api-only
```

or manually clone the repo and then run `npm install`.


### Docker

Create container

```
docker run \
    --name postgres \
    -e POSTGRES_PASSWORD=root \
    -e POSTGRES_USER=root \
    -e POSTGRES_DB=acladonis \
    -p 5432:5432 \
    -d \
    postgres
```

Starting when is offline:
ID Container = a46a366365bb (for me)
`docker start a46a366365bb`

### Migrations

Run the following command to run startup migrations.

```js
adonis migration:run
```
