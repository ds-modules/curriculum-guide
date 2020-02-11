# Building Instructions for Curriculum Guide

This is a guide intended to demonstrate how you can make edits to the curriculum guide on Github. The guide is built on [Jupyter Book](https://jupyter.org/jupyter-book/intro.html); see their website for detailed instructions on how to use it. This guide covers the basics and instructions specific to this repository.

## Step-By-Step

1. Begin by cloning the repository locally.
2. Make changes to files in the `content` folder. Pages and corresponding files can be found in [`data/_toc.yml`](data/_toc.yml). 
3. Add any new pages to [`data/_toc.yml`](data/_toc.yml).
4. Build the site from your terminal. If you're currently in the curriculum guide directory, run

```bash
make book
make build
```

5. \(Optional\) Run a docker server locally to view the changes before pushing. This can be run using the following terminal command from the curriculum guide directory:

```bash
$ rm Gemfile.lock
make serve
```

6. Commit the changes and push to Github.

More info on the docker server is on the [Jupyter Book website](https://jupyter.org/jupyter-book/guide/03_build.html#building-your-site-locally-with-containers-docker).
