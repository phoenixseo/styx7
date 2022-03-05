# Styx7
L.A.M.P. in a Container. Podman Container for Fedora Silverblue. LAMP-Stack with {Apache 2.4, PHP 7.4, Composer 2, git} to run as local development server for PHP-based Projects.

## Start Styx7

```
cd styx7/; sudo podman-compose up -d
```

## Stop Styx7

```
cd styx7/; sudo podman-compose down
```

## Why sudo?
Container shall use Host Network and priviledged Port 80.
Currently I don't know a better way to achive this goal.

## Host Config
See [Host-Config](../docs/host.md)

### Build by
PHOENIXSEO.de Frank Pfabigan e.K.
[https://phoenixseo.de](https://phoenixseo.de)
