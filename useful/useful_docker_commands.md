---
title: Useful Docker commands
layout: appleII
---

from command line
-----------------

```
docker ps -a

docker run hello-world

docker run --rm busybox date

docker run -i -t ubuntu /bin/bash

docker images

docker info

docker system prune

docker build .

docker build . -t image_tag_name

docker run --name container_name -d -p 4000:4000 image_tag_name

docker exec -it image_tag_name bash

docker stop container_name

docker compose up
```

resources
---------

[Docker: Remove All Images and Containers](https://davidwalsh.name/docker-remove-all-images-containers)
