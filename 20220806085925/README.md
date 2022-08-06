# Remove dangling images in docker
```bash
docker rmi -f $(docker images -f "dangling=true" -q
```

Tags:
```
#docker #dangle #dangling_image
```

Related
```
https://nickjanetakis.com/blog/docker-tip-31-how-to-remove-dangling-docker-images
```
