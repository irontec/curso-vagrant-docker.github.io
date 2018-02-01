## Dockerfile

Structure

```CoffeeScript
FROM debian:wheezy
MANTAINER Luis García <lfgarcia@irontec.com>

# Variables de entorno
ENV key value

# actualizar repositorio
RUN apt-get update

# Instalar mysql server
RUN apt-get install -y mysql-server

# Exponer el puerto 3306 (para enlaces entre contenedores)
EXPOSE 3306

# Volumeness
VOLUME /host/folder:/container/folder

# Copiar archivos
## ADD descomprime archivos tar.gz
ADD ./file_relative_to_dockerfile_in_host /container/file
ADD ./file_relative_to_dockerfile_in_host.tar.gz /container/folder

COPY ./file_relative_to_dockerfile_in_host.tar.gz /container/folder
COPY ./file_relative_to_dockerfile_in_host.tar.gz /container/file.tar.gz

# User 
USER vagrant

# Workdir
WORKDIR /opt
WORKDIR klear-development

# Entry Point (solo uno por Dockerfile)
ENTRYPOINT ["/user/bin/influxdb", "-config=/opt/influxdbconfig.toml"]
ENTRYPOINT supervisor

# command (solo uno por Dockerfile) (Se puede usar como parámetros de ENTRYPOINT)

CMD ["/usr/local/bin/diamond", "-f"]
CMD echo "This is a test. " | wc -
CMD ["--help"]

```

