# Python Packages

## Pre-installed Packages

Many Python packages have been pre-installed on JupyterHub and are available by default. You can `import` the desired package to start using it. [This](https://github.com/berkeley-dsep-infra/datahub/blob/prod/user-image/requirements.txt) file on GitHub contains a list of all the packages that are available by default.

## Installing New Packages

You can also install other packages that are not on this list. There are two methods for installation.

* **Temporary installation** - Notebooks provide support for bash commands in code cells. The line below, when run in a notebook code cell, will temporarily install numpy into a user's personal account. Numpy will then be available for use while the notebook is running. However, this cell must be rerun every time the notebook is started. Note, this is not a system-wide installation. Running the cell below will only install numpy temporarily into your personal account.  

```
!pip install numpy
```

* **Long-term installation** - You can contact us on Piazza if you want to install packages system-wide on datahub. These packages will then be available to all users by default and can be used with an `import` statement in all notebooks. You do not need to use the bash command shown above. **This is the recommend method for packages that will be used frequently. **



