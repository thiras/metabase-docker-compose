# metabase-docker-compose :whale: <!-- omit in toc --> 
This project aims to build a production ready docker-compose file for Metabase.

> [PR](https://github.com/thiras/metabase-docker-compose/pulls) are welcome. Contributors should comply with [code of conduct](https://github.com/thiras/metabase-docker-compose/blob/master/CODE_OF_CONDUCT.md).

# Table of Contents <!-- omit in toc --> 
- [Prepering](#prepering)
- [Run](#run)
- [Roadmap](#roadmap)

## Prepering
First, you need to create `.env` file;
```
cp .env.example .env
```

Then, you need to change passwords at `.env` file. Do not forget adjust `JAVA_TIMEZONE` environment according to your timezone. You should also adjust `PGADMIN_DEFAULT_EMAIL` variable with your email.

## Run
```
docker-compose up -d
```

and then point to `localhost:3000`. It may take couple of minutes to get a response until containers are up and running. You may use PgAdmin4 in case needed from `localhots:3001`.

## Roadmap
- [ ] MongoDB setup at the start
- [ ] Improve documentation
- [ ] Clustering?
- [ ] Inject sample data