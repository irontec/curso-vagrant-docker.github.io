#### Listar contenedores

```bash
$ docker ps
$ docker ps -a
$ docker ps --all
```

#### Crear contenedores

```bash
$ docker run debian:wheezy /bin/echo "Hello world"
$ docker run debian:wheezy /bin/sh -c "while true; do echo 'Hello world'; sleep 1; done"
$ docker run --rm debian:wheezy /bin/sh -c "while true; do echo 'Hello world'; sleep 1; done"
```
#### Terminal interactiva en un contenedor

```bash
$ docker run --rm -i -t debian:wheezy /bin/bash
$ docker run --rm -it debian:wheezy /bin/sh
```

#### Lanzar un contenedor como demonio

```bash
$ docker run -d --rm --name="debian_container" debian:wheezy /bin/sh -c "while true; do echo 'Hello world'; sleep 1; done"
```
