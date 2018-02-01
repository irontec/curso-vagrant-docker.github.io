#### Listar imágenes

```bash
$ docker images

REPOSITORY                                      TAG                            IMAGE ID            CREATED             SIZE
hello-world                                     latest                         f2a91732366c        2 months ago        1.85kB

$
```

#### Exportar imágenes

```bash
docker save -o image.tar repository|repository:tag|id 
docker save --output="image.tar" repository|repository:tag|id
```

```bash
$ docker save -o hello-world.tar hello-world:latest
$ ls -l

-rw-------   1 abejaruco abejaruco 12800 ene 31 22:51 hello-world.tar

```