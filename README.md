# A GitHub action to run docker-compose

You can find the image on [Docker Hub](https://hub.docker.com/r/blag/action-docker-compose)

[![Docker Pulls](https://img.shields.io/docker/pulls/blag/action-docker-compose.svg)](https://hub.docker.com/r/blag/action-docker-compose)

I use the base image [docker/compose](https://hub.docker.com/r/docker/compose) for this action

## Example usages

```yml
  - uses: actions/checkout@v4
  - name: run docker-compose
    uses: blag/action-docker-compose@latest
    with:
        # https://docs.docker.com/compose/reference/overview/
        cli-args: "build"

  - name: run docker-compose
    uses: blag/action-docker-compose@latest
    with:
        # https://docs.docker.com/compose/reference/overview/
        cli-args: "run my_image"

  - name: run docker-compose
    uses: blag/action-docker-compose@latest
    with:
        # https://docs.docker.com/compose/reference/overview/
        cli-args: "up"
```
