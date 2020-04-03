# portyx-env

#### hosts

```
127.0.0.1        portyx.local
127.0.0.1        api.portyx.local
127.0.0.1        sentry.portyx.local
```

#### setup
- pull images `docker-compose pull`

### Sentry setup
- generate secret key `docker-compose run --rm sentry config generate-secret-key`
- copy `.env-example` as `.env` and paste secret key
- up instance `docker compose up -d`
- run migrations `docker-compose run --rm sentry upgrade`
