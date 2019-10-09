# Hosting your course's content with Jupyter Book

![](https://jupyterbook.org/images/logo/logo.png)

Jupyter Book is a tool originally created here at Berkeley to create
open online textbooks for the content of Data 8. It is the tool used
to host the guide you're reading right now!

You can use Jupyter Book to create an online version of your own
course's content. To do so, check out the
[Jupyter Book documentation for building your own book](https://jupyterbook.org/guide/01_overview.html).

The basic steps to do so are as follows:

1. **Prepare your course's content**. Your content should be a collection of `.ipynb` and markdown
   files that are all in the came folder (usually called `_content/`).
2. **Create your Jupyter Book template**. This can be done by following
   [the steps outlined in the Jupyter Book guide](https://jupyterbook.org/guide/02_create.html).
3. **Configure your book**. This is done by editing the `_config.yml` file and creating your
   own Table of Contents file (in `_data/toc.yml`) to define your book structure.
3. **Build the HTML for your book's pages**. You need to convert each page (e.g., an `.ipynb` or `.md` file)
   into HTML so that we can serve it online. To do so, run the command:

   ```bash
   jupyter-book build path/to/mybook
   ```

   See the [build your book](https://jupyterbook.org/guide/03_build.html) documentation for
   more information.
4. **Host your book online**. There are a few ways to do this, one involving automatically
   building your book's website, and others that have you build it manually. Check out the
   [publishing your book online](https://jupyterbook.org/guide/04_publish.html) documentation
   for more information.

## Troubleshooting errors with Jupyter Book

If you're having a hard time figuring out how to build, configure, or publish your Jupyter Book,
please [open an issue on the Jupyter Book repository](https://github.com/jupyter/jupyter-book/issues/new).
