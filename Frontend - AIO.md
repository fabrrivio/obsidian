<h1>Communiquer nuxt avec l'aio locale</h1>
- changer la config dans docker-compose.yaml
  extra_hosts:
      - "back.aio-prm.aio:${DOCKER_HOST_IP}"
* changer le .env du projet
  AIO_API_BASE_URL=https://back.aio-prm.aio
  SITE_HOSTNAME=https://back.aio-prm.aio
* redemarrer docker

