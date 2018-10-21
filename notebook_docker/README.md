![docker pulls](https://img.shields.io/docker/pulls/jupyter/scipy-notebook.svg) ![docker stars](https://img.shields.io/docker/stars/jupyter/scipy-notebook.svg) [![](https://images.microbadger.com/badges/image/jupyter/scipy-notebook.svg)](https://microbadger.com/images/jupyter/scipy-notebook "jupyter/scipy-notebook image metadata")

# Jupyter Notebook Scientific Python Stack (README.md from the official website)

Please visit the documentation site for help using and contributing to this image and others.

* [Jupyter Docker Stacks on ReadTheDocs](http://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)
* [Selecting an Image :: Core Stacks :: jupyter/scipy-notebook](http://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-scipy-notebook)

# About this docker (and associated Makefile and bash scripts):

The `docker-compose.yml` file defines a notebook service (essentially creating a container
by using the `scipy-notebook` docker image). The current directory (the one with the
`docker-compose.yml` and `Makefile` etc...) will be mounted to the `/work` directory inside
the docker.

## To run the notebook container (and run jupyter notebook):
Use the bash command:
```bash
make up
```
Then open url that is provided, remember to copy in the token in the url.

## To shell into the container:
User the bash command:
```bash
make shell
```
Then you will enter the shell (bash) of the `scipy-notebook` container. To exit, type `exit` in
the docker shell.
