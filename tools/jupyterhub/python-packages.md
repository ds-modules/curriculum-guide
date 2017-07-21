# Python Packages

## Pre-installed Packages

Many Python packages have been pre-installed on JupyterHub and are available by default. You can `import` the desired package to start using it.

## Installing New Packages

You can also install other packages that are not on this list. There are two methods for installation:

* Temporary installation - Notebooks provide support for bash commands in code cells. The line below, when run in a notebook code cell, will temporarily install numpy. numpy will then be available for use while the notebook is running. However, this cell must be rerun every time the notebook is started. 

```
!pip install numpy
```

* Long-term - You can contact us on Piazza if you want to install packages on datahub. These packages will then be available by default and can be used with an `import` statement in all notebooks. You do not need to use the bash command shown above. **This is the recommend method for packages that will be used frequently. **



