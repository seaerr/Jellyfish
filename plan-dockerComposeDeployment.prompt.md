Plan for Docker Compose deployment:

- Copy the example environment file to `.env`:
  - `cp deploy/compose/.env.example deploy/compose/.env`
- Start Docker Compose with the provided environment file and compose YAML:
  - `docker compose --env-file deploy/compose/.env -f deploy/compose/docker-compose.yml up --build`
- Ensure Docker Desktop / Docker Engine is running before executing the command.
- If this is the first run, allow Docker to pull images and build any local services.
- Monitor the logs for startup errors and verify services become healthy.
