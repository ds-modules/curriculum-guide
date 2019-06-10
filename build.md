# Building Instructions for Curriculum Guide

This is a guide intended to demonstrate how you can make edits to the curriculum guide on Github. The guide is built on [Jupyter Book](https://jupyter.org/jupyter-book/intro.html); see their website for detailed instructions on how to use it. This guide covers the basics and instructions specific to this repository.

## Step-By-Step

1. Begin by cloning the repository locally.
2. Make changes to files in the `content` folder. Pages and corresponding files can be found in [`data/_toc.yml`](data/_toc.yml). 
3. Add any new pages to [`data/_toc.yml`](data/_toc.yml).
4. Build the site from your terminal. If you're currently in the curriculum guide directory, run
```bash
jupyter-book build .
```
5. \(Optional\) Run a docker server locally to view the changes before pushing. This can be run using the following terminal command from the curriculum guide directory:
```bash
$ rm Gemfile.lock
$ docker run --rm --security-opt label:disable -v /path/to/curriculum-guide:/srv/jekyll -p 4000:4000 -it -u 1000:1000 emdupre/jupyter-book bundle exec jekyll serve --host 0.0.0.0
```
Make sure that you edit the path to the curriculum guide. It should be a path from your home directory, not from wherever you are currently. More info on the docker server is on the [Jupyter Book website](https://jupyter.org/jupyter-book/guide/03_build.html#building-your-site-locally-with-containers-docker).
6. Commit the changes and push to Github.