#### Eliminar un contenedor

```bash
docker rm id|name
```

```bash
$ docker rm ngingx_curso
```

#### Crear una imagen a partir de un contenedor

```bash
docker commit id|name [registry/]user/image[:tag]
```

```bash
$ docker commit ngingx_curso abejaruco/nginx:custom
```

#### Subir imagen a Docker Hub

```bash
docker push user/image[:tag]
```

```bash
$ docker push abejaruco/nginx:custom
```