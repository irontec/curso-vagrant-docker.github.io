#### Importar imágenes

```bash
docker load -i hello-world.tar
docker load --input="hello-world.tar"
```

```bash
$ docker load -i hello-world.tar
$ docker load --input="hello-world.tar"

f999ae22f308: Loading layer [==================================================>]  3.584kB/3.584kB
Loaded image: hello-world:latest
$ docker images

REPOSITORY                                      TAG                            IMAGE ID            CREATED             SIZE
hello-world                                     latest                         f2a91732366c        2 months ago        1.85kB
```

