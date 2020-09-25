+++
title = "converting jupyter notebooks to org mode"
author = ["Cameron Smith"]
lastmod = 2020-09-25T02:08:01-04:00
slug = "converting_jupyter_notebooks_to_org_mode"
draft = false
+++

## introduction {#introduction}


### use case {#use-case}


### tests {#tests}

It will be helpful to use a relatively simple jupyter notebook. I will use the `ipynb` for testing nbcorg and the jupytext markdown for testing pandoc conversion.


## tools {#tools}


### pandoc {#pandoc}

It might make more sense to just use `pandoc` from the command line; however, there is a package named `org-pandoc-import` that allows for importing these files directly from emacs. The doom config is

```text
(package! org-pandoc-import
  :recipe (:host github
           :repo "tecosaur/org-pandoc-import"
           :files ("*.el" "filters" "preprocessors")))
```

After loading that you just open the `ipynb` and then run the function `org-pandoc-import-to-org`. This works!


### nbcorg for nbconvert {#nbcorg-for-nbconvert}

reference :: [nbcorg · PyPI](https://pypi.org/project/nbcorg/)

Make sure we have the package installed.

```sh
echo $HOME $0
pwd
```

```text
/Users/crs58 /bin/sh
/Users/crs58/projects/notes/org
```

```sh
pip freeze | grep nbcorg
pip install nbcorg
```

Create directory and copy files for running the test.

```sh
PROJECT_DIR=~/projects/convert-jupyter-org
SOURCE_DIR=~/projects/applied-probabilistic-inference
mkdir -p $PROJECT_DIR
cp $SOURCE_DIR/plotting.* $PROJECT_DIR
ls $PROJECT_DIR
```

```text

sh-3.2$ sh-3.2$ sh-3.2$ plotting.ipynb	plotting.md	plotting.org	plotting.py
```

```sh
echo $PROJECT_DIR
echo $SOURCE_DIR
```

```text
/Users/crs58/projects/convert-jupyter-org
/Users/crs58/projects/applied-probabilistic-inference
```

```sh
cd $PROJECT_DIR
jupyter nbconvert --to orgmode --OrgmodeExporter.src_block_options=':session plotting :results output replace' --OrgmodeExporter.exclude_output=True plotting.ipynb
# jupyter nbconvert --version
```

Good to know that this is essentially broken for now due to

```text
File "/Users/crs58/.asdf/installs/python/3.8.2/lib/python3.8/site-packages/jinja2/loaders.py", line 429, in load
  raise TemplateNotFound(name)
jinja2.exceptions.TemplateNotFound: base.tpl
```
