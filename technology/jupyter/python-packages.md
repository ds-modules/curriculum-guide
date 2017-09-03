# Python Packages

### Pre-installed Packages

Many Python packages have been pre-installed on JupyterHub and are available by default. [This file on GitHub](https://github.com/berkeley-dsep-infra/datahub/blob/prod/user-image/requirements.txt) contains a list of all the packages \(and corresponding versions\) that are available by default. To use a pre-installed package such as `numpy`, you can simply type the line below into a code cell.

```
import numpy
```

### Installing New Packages

You can also install other packages that are not on this list. There are two methods for installation. If you will be using a package regularly in your course, we recommend using the long-term installation method.

##### Temporary installation

Notebooks provide support for bash commands in code cells. The line below, when run in a notebook code cell, will temporarily install `numpy` into a user's personal account. `numpy` will then be available for use while the server is running. This cell must be run every time the user's server is restarted. Note, this is not a system-wide installation. Running the cell below will only install numpy temporarily into a user's personal account.

```
!pip install numpy
import numpy
```

##### **Long-term installation**

You can contact us on Piazza if you want to install packages system-wide on DataHub. These packages will then be available to all users by default and can be used with an `import` statement in all notebooks. For example, `numpy` is pre-installed, you can just type the line below into a code cell, without first having to install `numpy`. **This is the recommend method for packages that will be used frequently. **

```
import numpy
```



