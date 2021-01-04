> This project is part of the [clevr-compose-stacks](...). Instructions below assume existing instance of the [traefik-stack](...) has been setup. [Learn more...](...)

---

# hugo

Docker image containing hugo, based off of [klakegg/hugo](https://hub.docker.com/r/klakegg/hugo/) which runs `hugo server` by default using this sample site:

https://github.com/wowchemy/starter-academic

---

## Configure

* Edit the docker-compose environment file `.env`

## Build

Building the image locally is only required if changes to the image are made.

```bash
docker-compose -f image/docker-compose.build.yml build
```

Publish changes to Docker registry:

```bash
docker-compose -f image/docker-compose.build.yml push
```

## Start

```bash
# attached
docker-compose up

# or detached
docker-compose up -d
```

## Use

Access the app in your browser according to variables set in the environment file (`.env`): `https://<APP_DNS_NAME>.<DNS_DOMAIN>`; e.g., `https://blog.clevrdev.com`.

## Support

TODO: Links
