# Reomve untaged docker images
```bash
docker rmi $(docker images --filter "dangling=true" -q --no-trunc)
```

Tags:
```
#docker #dangeling #unsued_images #none_tag
```

Related
```
* https://docs.docker.com/config/pruning/
* https://docs.docker.com/engine/reference/commandline/image_prune/
* https://stackoverflow.com/questions/32723111/how-to-remove-old-and-unused-docker-images
```
