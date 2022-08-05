# Steps to Launch Jupyter Notebooks using RetroLab interface

RetroLab is an alternative JupyterLab distribution, built from the ground-up, providing a notebook interface with a retro look and feel. RetroLab provides the 
retro interface similar to Classic Notebooks while retaining some of the advanced features from JupyterLab which includes extensions/plugins. 
If you want to learn more about RetroLab, then please do checkout Jeremey Tuloup's wonderful documentation [here](https://blog.jupyter.org/retrolab-a-jupyterlab-distribution-with-a-retro-look-and-feel-8096b8b223d0).

We recommend using RetroLab interface to launch Jupyter notebooks for the following reasons,
- Classic notebook interface is going to be deprecated in the next few months due to the complexity of maintaining the codebase. The Classic Notebook release 7.0 will have retrolab as the defaul editor to launch notebooks.
- Latest accessibility related changes are only happening in JupyterLab and RetroLab.


# Step 1
Access nbgitpuller plugin and select "RetroLab" option from the "Open In" dropdownlist.

```{figure} ../images/retrolab_nbgitpuller.PNG
:width: 500px
:align: center
:name: Launch RetroLab

Here is how you instruct nbgitpuller plugin to create a link that launches notebooks in RetroLab
```

# Step 2
Paste the nbgitpuller link in the browser inorder to launch the notebooks using RetroLab in Datahub

```{figure} ../images/retrolab_interface.gif
:width: 500px
:align: center
:name: RetroLab interface

Here is how the notebooks get rendered in RetroLab interface
```

# Step 3
Identify required extensions from JupyterLab and install them in RetroLab. If you have trouble installing any third party extensions then please do reach out to us so that we can figure out a solution for the same.






