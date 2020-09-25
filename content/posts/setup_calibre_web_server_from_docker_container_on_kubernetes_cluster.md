+++
title = "setup calibre web server from docker container on kubernetes cluster"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:37:42-04:00
slug = "setup_calibre_web_server_from_docker_container_on_kubernetes_cluster"
draft = false
+++

## <https://hub.docker.com/r/linuxserver/calibre-web> {#https-hub-dot-docker-dot-com-r-linuxserver-calibre-web}


## Docker compose snippet {#docker-compose-snippet}


### \`\`\`clojure {#clojure}

---
version: "2.1"
services:
  calibre-web:
    image: linuxserver/calibre-web
    container\_name: calibre-web
    environment:

<!--list-separator-->

-  PUID=1000

<!--list-separator-->

-  PGID=1000

<!--list-separator-->

-  TZ=Europe/London

<!--list-separator-->

-  DOCKER\_MODS=linuxserver/calibre-web:calibre

    volumes:

<!--list-separator-->

-  path to data:/config

<!--list-separator-->

-  path to calibre library:/books

    ports:

<!--list-separator-->

-  8083:8083

        restart: unless-stopped
    \`\`\`


## What's the best backend to substitute in the "path to data" for kubernetes? {#what-s-the-best-backend-to-substitute-in-the-path-to-data-for-kubernetes}


##  {#}
