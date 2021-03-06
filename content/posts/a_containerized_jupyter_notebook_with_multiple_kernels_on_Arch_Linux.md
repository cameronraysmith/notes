+++
title = "a containerized jupyter notebook with multiple kernels on Arch Linux"
author = ["Cameron Smith"]
lastmod = 2020-11-30T00:41:57-05:00
slug = "a_containerized_jupyter_notebook_with_multiple_kernels_on_Arch_Linux"
draft = false
+++

## references {#references}

-   github: <http://github.com/cameronraysmith/notebooks>
-   dockerhub: <https://hub.docker.com/repository/docker/cameronraysmith/notebooks>
-   arch linux on GCP
    -   <https://github.com/GoogleCloudPlatform/compute-archlinux-image-builder/blob/master/build-arch-gce>


## readme {#readme}

<!--list-separator-->

-  notebooks

    About

    See the Makefile for relevant commands.

    File listing

    ```text
        ▶ tree -I 'maxima-jupyter'
        .
        ├── Dockerfile
        ├── Makefile
        ├── README.md
        ├── VERSION
        ├── etc
        │   ├── jupyter_notebook_config.py
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
    ```

    LICENSE

    This code is distributed under the [MIT License](http://opensource.org/licenses/MIT).


## doom emacs {#doom-emacs}

-   should put a custom version of my `doom.d` directory into the default `dotfiles-local` of the `notebooks` repository which should eliminate the steps below
    -   needed to have `cmake` installed so this should be added to packages
    -   realized that I needed `wget` to download [doom black hole image](https://github.com/hlissner/doom-emacs/issues/2204#issuecomment-626654221), which doesn't get used properly but would probably lead the config to cause an error
    -   had to add paths such as `~/projects/notes/org/private/agenda`,  `~/org/bib/`, `~/Downloads/figures/` for compatibility with my `doom.d` configuration
    -   had to clone my `dotfiles-local` repository and then copy the `doom.d` directory into the remote machine's copy of `dotfiles-local`, run `rcup`, and then run `emacs.d/bin/doom sync`.
-   had to use `SPC :` to call `M-x`
-   had to hard link any shared github repositories containing org files into `projects/notes/org/`
-   used `global-command-log-mode` and set `command-log-mode-window-size` to `60` instead of `40`
