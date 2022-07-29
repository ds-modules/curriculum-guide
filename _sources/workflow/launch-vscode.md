# Launching notebooks using VSCode in Datahub

# Step 1

## Generate nbgitpuller links to launch via vscode editor

- Access ngbitpuller link generator website  - https://jupyterhub.github.io/nbgitpuller/link
- Enter https://eecs.datahub.berkeley.edu as the JupyterHub URL
- Enter your Git repository having source files as Git Repository URL
- Enter your source file branch as part of the "branch" field
- For "Application to Open" option, Enter Custom URL as "vscode/?folder=<Your folder structure>"

```{figure} ../images/vscode_link_generator.PNG
:width: 500px
:align: center
:name: nbgitpuller link to launch VSCode

Here is how you can generate a link to launch vscode in EECS Hub
```

Copy the unique link that is generated and paste it in your browser. VSCode editor gets launched in the browser showing the required repository as part of the home directory.

# Step 2

## Configure VSCode to launch notebooks with python extensions preinstalled

- Find the python notebook file (ipynb) that you want to launch in vscode editor directory space
- Execute the cell which contains the code to install python packages
- Incase if you are not able to run a particular cell, check if python extension is pre-installed. 
- If it is not installed, Search "python" in the extension list and install "ms-python" extension directly or click this [link](https://open-vsx.org/extension/ms-python/python) to install the python extension.
- In addition, Search "Jupyter" in the extension list and install "ms-toolsai.jupyter" extension directly or click this [link](https://open-vsx.org/extension/ms-toolsai/jupyter) to install the Jupyter notebook extension.


```{figure} ../images/python_extension.PNG
:width: 500px
:align: center
:name: Install Python extension

Install python extension in the notebook
```

# Step 3

## Run Otter grader in VSCode

- For installing Otter grader, there are no extra steps. Ensure that you complete the step 1 and 2 and pip install otter-grader before you execute the cell containing the code.


