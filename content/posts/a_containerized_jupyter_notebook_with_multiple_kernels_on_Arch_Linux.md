+++
title = "a containerized jupyter notebook with multiple kernels on Arch Linux"
author = ["Cameron Smith"]
lastmod = 2020-09-24T22:41:11-04:00
slug = "a_containerized_jupyter_notebook_with_multiple_kernels_on_Arch_Linux"
draft = false
+++

## <http://github.com/cameronraysmith/notebooks> {#http-github-dot-com-cameronraysmith-notebooks}


### readme {#readme}

<!--list-separator-->

-  notebooks

    About

    See the Makefile for relevant commands.

    File listing

    \`\`\`bash
    ▶ tree -I 'maxima-jupyter'
    .
    ├── Dockerfile
    ├── Makefile
    ├── README.md
    ├── VERSION
    ├── etc
    │   ├── jupyter\_notebook\_config.py
    │   ├── pkglist-01.txt
    │   ├── pkglist-02.txt
    │   ├── pkglist-startup.txt
    │   ├── pkglist-yay.txt
    │   └── python-libraries.txt
    ├── notebooks
    │   ├── ...
    │   └── common-lisp-jupyter
    │       ├── ...
    ├── scratch
    │   ├── scraps.dockerfile
    │   └── scraps.mk
    └── scripts
        └── startup.sh
    \`\`\`

    LICENSE

    This code is distributed under the [MIT License](http://opensource.org/licenses/MIT).


## <https://hub.docker.com/repository/docker/cameronraysmith/notebooks> {#https-hub-dot-docker-dot-com-repository-docker-cameronraysmith-notebooks}


## <https://github.com/GoogleCloudPlatform/compute-archlinux-image-builder/blob/master/build-arch-gce> {#https-github-dot-com-googlecloudplatform-compute-archlinux-image-builder-blob-master-build-arch-gce}
