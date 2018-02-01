#### Ver los logs de un contenedor

```bash
docker logs id|name
```

```bash
$ docker logs ngingx_curso
$ docker logs -f ngingx_curso
$ docker logs -f --tail 10 ngingx_curso
```


#### Obtener la información de un contenedor

```bash
docker inspect id|name
```

```bash
$ docker inspect ngingx_curso
```

#### Parar un contenedor

```bash
docker stop id|name
```
```bash
$ docker stop ngingx_curso
```

#### Arrancar un contenedor

```bash
docker start ngingx_curso
```

```bash
$ docker start ngingx_curso
```

notes:

Hablar de como funcionan los logs, que todo tiene que salir a stdout y stderror

Explicar un poco la información del contenedor con el inspect
