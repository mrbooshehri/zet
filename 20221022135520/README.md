# docker entrypoint.sh

```bash
#!/bin/bash
set -e

... code ...

exec "$@"
```

```set -e``` sets a shell option to immediately exit if any command
being run exits with a non-zero exit code. The script will return with
the exit code of the failing command.

```exec "$@"``` is typically used to make the entrypoint a pass through
that then runs the docker command. It will replace the current running
shell with the command that "$@" is pointing to. By default, that
variable points to the command line arguments.

Tags:
```
#docker #dockerfile #entrypoint #entrypoint.sh
```

Related:
```
* https://stackoverflow.com/questions/39082768/what-does-set-e-and-exec-do-for-docker-entrypoint-scripts
```
