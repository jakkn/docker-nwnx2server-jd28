# docker-nwnx2server-jd28
Containerization of NWNX2 server on Linux from jd28's fork that supports [nwnx-haks](https://github.com/jd28/nwnx-haks)

Base on [docker-nwnserver](https://github.com/jakkn/docker-nwnserver), with [docker-nwnx2server](https://github.com/jakkn/docker-nwnx2server) as a boilerplate.

## Run
```
docker-compose up -d
```

#### Note
Options to nwserver can be given in the following ways:
- Using `docker-compose.yml` the default script can be changed to `compose-nwnstartup.sh` and will pass on any arguments from the compose file to nwserver. This is the recommended procedure.
- Using the default script `nwnstartup.sh`. This will try to load a module named `module.mod`

The plugin nwnx_jvm has been skipped due to compile issues.

## Dependencies
- [Docker](https://docs.docker.com/engine/installation/)
- [Compose](https://docs.docker.com/compose/install/)

## References
[NWNX2](https://github.com/nwnx/nwnx2-linux)
