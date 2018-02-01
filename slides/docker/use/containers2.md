#### Exponer puertos

```bash
docker run -p host_port:container_port image command
docker run -P image command
```

```bash
$ docker run --rm nginx
$ docker run --rm -p 8080:80 nginx
$ docker run --rm -P nginx
```

#### Compartir Volúmenes

```bash
docker run -v /host/folder:/container/folder image command
```

```bash
$ docker run -d -v ${PWD}:/usr/share/nginx/html -p 8080:80 --name="ngingx_curso" nginx
```

Más opciones del comando docker run
```bash
$ docker run --help
```

notes:

"-P" expone los puertos al azar.


Compartir un volumen con una carpeta vacía y cuando
ya esté el contenedor corriendo crear el index.html

Esta compartición no penaliza como en virtual box.

