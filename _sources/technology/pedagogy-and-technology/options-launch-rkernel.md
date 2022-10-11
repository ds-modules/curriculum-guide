# Backup options to Launch R notebooks

If you are a user who cannot access Datahub due to the following reasons, 
- You don't have a Calnet log-in currently or
- You are not able to access the Datahub service as it is down
then you can explore the below mentioned options to launch R notebooks.

### Option #1: Launch Jupyter R Kernel locally

Step 1: Install Anaconda distribution (JupyterLab application gets installed through this process) locally in your device. Check this [link](https://docs.anaconda.com/anaconda/install/index.html) for the installation process.

Step 2: Open Anaconda prompt shell. Run the following code to install R Kernel in Jupyter Lab,

```{code}
conda install -c r r-essentials
```

```{note}
Press "y" when command line prompts
```

Step 3: Run the following command to install tidyverse.

```{code}
conda install -c r r-tidyverse
```

```{note}
Press "y" when command line prompts to install all the packages
```

Step 4: Run the following command to launch Jupyter Lab

```{code}
jupyter lab
```

Step 5: Now, from the launcher tab, choose R kernel to start a new notebook.

```{figure} ../../images/launcher_tab_r_kernel.jpg
:width: 500px
:align: center
:name: Jupyter Notebook Launcher Tab with R Kernel
```

The following is a screenshot of Jupyter notebook having R kernel.

```{figure} ../../images/jupyter_notebook_r_kernel.jpg
:width: 500px
:align: center
:name: Jupyter Notebook with R Kernel
```

### Option #2: Use Google Colab to launch R Kernel

Step 1: Launch R Kernel in Google Colab by accessing this [link](https://colab.to/r)

Step 2: Check whether the tidyverse packages (or any other package you need) are already installed in Colab by using the following code,

```{code}
print(installed.packages())
```

Step 3: If not installed, Install tidyverse package using the following command

```{code}
devtools::install_github("tidyverse/tidyverse")
```

### Option #3: Launch R notebooks using Binder

If you want a hosted Jupyterhub experience to launch your R notebooks then Binder is an option. Binder allows creating R notebooks in an executable environment. Launch [Jupyter R notebook](https://notebooks.gesis.org/binder/jupyter/user/binder-examples-r-conda-ofu958y9/lab) or [R Studio](https://mybinder.org/v2/gh/binder-examples/r-conda/master?urlpath=rstudio) using the shared binder links.

### Option #4: Launch R notebooks using R Studio

If you are a RStudio fan, you can access [RStudio Cloud](https://rstudio.cloud/plans/instructor) where you can purchase a hosted environment for your coursework.

```{note}
Students need to create R Studio accounts.
```

If you don't plan to purchase an R Studio cloud account, you can ask students to download and install a free [RStudio Desktop application](https://www.rstudio.com/products/rstudio/) on their desktop.