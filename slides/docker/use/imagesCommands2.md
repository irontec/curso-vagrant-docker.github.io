#### Eliminar imágenes

```bash
docker rmi repository|repository:tag|id
```

```bash
$ docker rmi hello-world
$ docker rmi  hello-world:latest
$ docker rmi f2a91732366c

Error response from daemon: conflict: unable to remove repository reference "hello-world:latest" (must force) - container da880982fe2b is using its referenced image f2a91732366c

$ docker rmi  --force hello-world:latest
$ docker rmi  -f hello-world:latest

Untagged: hello-world:latest
Untagged: hello-world@sha256:66ef312bbac49c39a89aa9bcc3cb4f3c9e7de3788c944158df3ee0176d32b751
Deleted: sha256:f2a91732366c0332ccd7afd2a5c4ff2b9af81f549370f7a19acd460f87686bc7

$ docker images

REPOSITORY                                      TAG                            IMAGE ID            CREATED             SIZE
$ 

```