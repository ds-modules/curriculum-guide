# Creating Notebooks

Below is an short introduction on how to Jupyter notebooks on `datahub.berkeley.edu`. Assignment development can be done on `datahub.berkeley.edu` or locally, if you already have a local Jupyter setup. The below steps assume you are working on DataHub, but most of the steps can be done on a local setup as well. If you decide to work locally, we recommend you test your notebooks on `datahub.berkeley.edu` well in advance. The development environment on DataHub is probably different from your local environment, so it is possible that code may break.

## Create a Blank Notebook

This section describes how to create a notebook on the JupyterHub infrastructure. Go to [datahub.berkeley.edu](https://datahub.berkeley.edu). Click on the green `Start My Server` button. You will not need to do this if you are working locally.

![](https://cloud.githubusercontent.com/assets/8205702/23236423/0ae83eb6-f90e-11e6-9c17-8d4f0eff9408.png)

Click on the `New` dropdown on the right side of the page. Select the option for `Python 3` under `Notebooks`.

![](https://cloud.githubusercontent.com/assets/8205702/23236478/4418c61a-f90e-11e6-8b2a-42c3ab52f423.png)

You will see a blank notebook to which you can now add text and code. The notebook consists of sections called cells. There are different types of cells that can be used. Code is part of the "code" cell type and text is part of the "markdown" cell types.

## Add a New Cell

You can add a new cell using eiher the `+` button on the left side or the `Insert` button on the toolbar.

![](https://cloud.githubusercontent.com/assets/8205702/23236603/a1ff8b9c-f90e-11e6-947e-a99c33d9bbe4.png)

To set the type of this cell, click on `Cell` in the toolbar, then `Cell Type` and then either `Code` or `Markdown`. Code can be directly typed in. Text must be added in markdown format.

![](https://cloud.githubusercontent.com/assets/8205702/23236602/a1fc6f52-f90e-11e6-9749-c5dc2f73e172.png)

Here is an example of what code and markdown cells with content will look like.

![](https://cloud.githubusercontent.com/assets/8205702/23251037/8ede3e6c-f960-11e6-8699-cd0ff562e1e8.png)

You will notice that there is no code output in the previous image. In addition, the text formatting is not properly displayed. To run code or see the formatted text, you must run the cell. An individual cell can be run by typing Shift-Enter from the cell. All cells can be run by clicking the play button in the toolbar \(triangle with a line\). You can also click on "Cell" in the toolbar for additional ways to run cells. Below is the output of running all cells.

![](https://cloud.githubusercontent.com/assets/8205702/23251108/dcada876-f960-11e6-9629-ac8a1bdbe116.png)

## Run Code

You can run code by either typing Shift-Enter from the cell or clicking the play button in the toolbar \(triangle with a line\).

![](https://cloud.githubusercontent.com/assets/8205702/23251184/2e1be7fe-f961-11e6-9c84-e1b966c3e06b.png)

Code that has been run in one cell is accessible by another cell.  If any changes are made to a cell, you must rerun all cells that you want affected by the change.

![](https://cloud.githubusercontent.com/assets/8205702/23251192/394dfd9c-f961-11e6-8bef-d1aa93c18dec.png)

## Download Notebooks

Click on `File` in the toolbar, then `Download as`, then select `Notebook (.ipynb)` . This will download the notebook to your computer in the standard Jupyter notebook format. You can also download notebooks in alternate formats, seen below.

![](https://cloud.githubusercontent.com/assets/8205702/23284842/8995ced4-f9e2-11e6-809e-2b46bd7833da.png)

## Additional Resources

* [Markdown basics notebook](http://datahub.berkeley.edu/user-redirect/interact?repo=connector-instructors&path=examples/external_notebooks/markdown_basics.ipynb) - Double clicking on each cell allows you to see how a variety different content is formatted in Jupyter Notebooks.



