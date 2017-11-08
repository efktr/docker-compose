# docker-compose
This repository is dedicated to composing all pieces of the tool to be serviced via docker-compose


## Instructions

1. Clone this repo where you want to `docker-compose` the efktr services.
1. Change the `VIRTUAL_HOST` environment variables in the compose file to the hostnames where your applications will be living!
1. `docker-compose pull && docker-compose up -d`

**Note**: The `backend` image might fail to load up the first run, because the `data` container needs to import data and restart before being available. If that's the case you will need to re-start the `backend` container by simply running `docker-compose up -d` again.
