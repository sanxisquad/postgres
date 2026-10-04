# postgres (compartit)

Instància `postgres:16-alpine` per a serveis a `projectes_network`. **TracksMaint no la fa servir** (té MariaDB).

Compose: `docker-compose.yml`. Credencials: `.env` (no git). Port host: `127.0.0.1:5432`. Dades: volum `postgres_data`.

```bash
docker compose up -d
```

Consumidor actual: `../control-plane` (crear rol/DB a mà; veure `../infraestructura.md`).

No esborris el volum ni canviïs `container_name: postgres` sense actualitzar els altres composes.
