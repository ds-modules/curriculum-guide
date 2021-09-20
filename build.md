# Building Instructions for Curriculum Guide

This is a guide intended to demonstrate how you can make edits to the curriculum guide on Github. The guide is built on [Jupyter Book](https://jupyter.org/jupyter-book/intro.html); see their website for detailed instructions on how to use it. This guide covers the basics and instructions specific to this repository.

## Step-By-Step

1. Begin by cloning the repository locally.
2. Make changes to files in the `content` folder. Pages and corresponding files can be found in [`_toc.yml`](_toc.yml). 
3. Add any new pages to [`_toc.yml`](_toc.yml).
4. Build the site from your terminal. If you're currently in the curriculum guide directory, run

```bash
jupyter-book build curriculum-guide
```
5. Commit the changes and push to Github.
