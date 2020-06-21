# abme-env

#### hosts

```
127.0.0.1        abme.local
127.0.0.1        api.abme.local
127.0.0.1        sentry.abme.local
```

#### sentry setup
- copy `.env-example` as `.env` and paste secret key
- generate secret key `docker-compose run --rm sentry config generate-secret-key`
- run migrations `docker-compose run --rm sentry upgrade`
