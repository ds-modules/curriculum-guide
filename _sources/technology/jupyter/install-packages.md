# Package Installation in Python and R

**What are the packages pre-installed for every hub?**

Procedure for package installation varies across different programming languages. Basic python packages such as numPy, pandas, scikit-learn, matplotlib, etc., are installed across the main Datahub. R hubs supports packages such as shiny, dplyr, tidyR, RSQLlite, etc. However, you can customize the packages for the hubs by requesting them using this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=datahub-package-addition---change-request.md&title=Request+python+package+X+for+class+Y).
If you want to check the list of packages installed,
- You can use the below command for Python,

```python
!pip list
```
- You can use the below command for R,

```python
installed.packages()
```
- You can check the packages installed in Julia by accessing the [Julia Hub](http://julia.datahub.berkeley.edu/)

```{note}
Here is the [list](https://github.com/berkeley-dsep-infra/datahub/blob/staging/deployments/datahub/images/default/requirements.txt) of Python packages installed in datahub.berkeley.edu. Here is the [list](https://github.com/berkeley-dsep-infra/datahub/blob/staging/deployments/datahub/images/default/install.R) of R packages installed in datahub.berkeley.edu. Here is the [list](https://github.com/berkeley-dsep-infra/datahub/blob/staging/deployments/julia/image/install-julia-packages.jl) of Julia packages installed in datahub.berkeley.edu.
```

**What should I do if I want to install more packages?**

- Use your datahub instance to install the required version of the package. Self installation of packages in your instanceof hub is a temporary measure to identify dependencies. If you require a permanent solution then you need to [request](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=datahub-package-addition---change-request.md&title=Request+python+package+X+for+class+Y) us to install the required package(s) in your hub.

- If you want to install packages for Python in your instance, then use the following syntax,

```python
pip install <package-name>
Eg: pip install numpy
```

- If you want to install packages for R in your instance, then use the following syntax,

```python
install.packages("<package-name>")
install.packages("ggplot2")
```
- Check if there are specific dependencies for the installed package. Highlight the package name along with their version and dependencies as part of your [request](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=datahub-package-addition---change-request.md&title=Request+python+package+X+for+class+Y).

- Raise a request using this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=datahub-package-addition---change-request.md&title=Request+python+package+X+for+class+Y)!

### Pre-installed Packages

Many Python packages have been pre-installed on JupyterHub and are available by default. [This file on GitHub](https://github.com/berkeley-dsep-infra/datahub/blob/prod/user-image/requirements.txt) contains a list of all the packages \(and corresponding versions\) that are available by default. To use a pre-installed package such as `numpy`, you can simply type the line below into a code cell.

```
import numpy
```

### Installing New Packages

You can also install other packages that are not on this list. There are two methods for installation. If you will be using a package regularly in your course, we recommend using the long-term installation method.

#### Temporary Installation

Notebooks provide support for bash commands in code cells. The line below, when run in a notebook code cell, will temporarily install `numpy` into a user's personal account. `numpy` will then be available for use while the server is running. This cell must be run every time the user's server is restarted. Note, this is not a system-wide installation. Running the below cells will only install numpy and ggplot2 temporarily into a user's personal account.

```
!pip install numpy
import numpy
```

```
install.packages("ggplot2")
library("ggplot2")
```

#### **Long-term installation**

_This is the recommended method for packages that will be used frequently._

Our JupyterHub is deployed from the [berkeley-dsep-infra/datahub](https://github.com/berkeley-dsep-infra/datahub) GitHub repository. The `staging` branch reflects the state of the [staging hub](https://staging.datahub.berkeley.edu) while the `prod` branch reflects the state of the [production hub](https://datahub.berkeley.edu).

To request additional libraries in the [user environment,](https://github.com/berkeley-dsep-infra/datahub/tree/staging/deployments/datahub/image), [create an issue](https://help.github.com/en/articles/creating-an-issue) on the GitHub repo for DataHub (linked above); make sure to use the "DataHub Package Addition / Change Request" template.

<!-- 

Once this is complete and if there are no problems, you can request that someone review the PR before merging, or you can merge yourself if you are confident. This merge will trigger a continuous integration process on CircleCI that can be [observed live](https://circleci.com/gh/berkeley-dsep-infra/datahub/). This process upgrades the staging hub. Test your changes there when it is complete because we do not want unverified changes to linger in staging. For example if you updated a library, make sure that a new user server instance has the new version.

If staging fails, _never_ update production. Revert your change or call in help if necessary. If your change is successful, you will need to merge the change from staging branch to production. Create another PR, this time with the `base` set to prod and the `head` set to staging. This PR will trigger a similar continuous integration process. Test your change on production for good measure.

-->

##### On reproducibility

Make sure to specify a version for any library you install. If you do not, it is likely that the deployment process will break at some point during the semester. Omitting a version will not enable the user environment to always have the latest version -- it will only have the latest version that existed on the date that CI process runs. If you want to use an unreleased version of a library, specify the corresponding git SHA of that library's repository.