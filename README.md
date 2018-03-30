# dockerfiles
require: docker v17.*

## Scrapy Service
docker image automated build to: https://hub.docker.com/r/franten/scrapy/

networks: backend

## Postgres Service
docker image from: https://hub.docker.com/r/_/postgres/

volumes: postgres-db
networks: backend
