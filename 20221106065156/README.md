# Difference Between Docker Save and Export

The save command preserves the image layer information, including all
history and metadata. This allows us to fully import the tar file into
any Docker registry and use it to start new containers.

Conversely, the export command does not preserve this information. It
contains the same files as the image that started the container but
without history and metadata.

Additionally, the export command includes changes made while the
container was running, such as a new or modified file. This means
different containers from the same image may produce different tar files
when exporting them.

## Docker Images vs. Container

A Docker image is a file that contains all the files necessary to run an
application. This includes all of the operating system files, as well as
application code and any required supporting libraries.

A Docker container is a Docker image that has been started. A container
is essentially a running application. Containers consume memory and CPU
resources like a normal process and can also access file systems and
communicate with other containers via network protocols.

## Docker save

The Docker save command is used to save a Docker image to a tar file.
This command is helpful for moving a Docker image from one registry to
another or simply examining the contents of the image using the Linux
tar command.

```bash
docker save IMAGE > /path/to/file.tar
# or
docker save -o /path/to/file.tar IMAGE
```

## Docker Export

The Docker export command is used to save a Docker container to a tar
file. This includes both the image files as well as any changes made
while the container was running.

```bash
docker export CONTAINER > /path/to/file.tar
# or
docker export -o /path/to/file.tar CONTAINER
```

Tags:
```
#docker #save #export #docker_save #docker_export
```

Related:
```
* https://www.baeldung.com/ops/docker-save-export
```
