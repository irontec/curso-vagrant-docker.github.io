## ¿Qué es?

* Archivo de texto.
* Contiene comandos.
* Automatiza la creación de imágenes.

```bash
$ docker build .
$ docker build -t shykes/myapp .
```

* Cada comando se ejecuta de manera independiente.
* Por cada comando se crea una imágen intermedia (capa).