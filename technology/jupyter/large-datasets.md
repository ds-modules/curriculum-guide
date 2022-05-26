# Storing Datasets

A few methods of storing datasets are outlined below. The choice of method depends on your preference and the size of the dataset. Keep in mind, regardless of the size of your dataset, each account on DataHub is provided with ~1GB RAM, so this will limit the amount of data that you can read in at any time. If you want to temporarily increase this limit on RAM, please raise a [github issue](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=higher-resources.md&title=Request+more+RAM+for+class+X).

### Small Datasets \(a few MBs\)

##### GitHub

Datasets and the corresponding Jupyter Notebook can be stored in a folder on GitHub. You can then create a nbgitpuller link for the entire folder. When students click this link, the entire folder will appear on their JupyterHub account.

##### Outside Hosts

You can store the data on an online host such as Box, Google Drive, or even GitHub. The `datascience` package contains a [read\_table\(\)](http://data8.org/datascience/_autosummary/datascience.tables.Table.read_table.html#datascience.tables.Table.read_table%29\) function for the [Tables](http://data8.org/datascience/tables.html%29\) data structure. This function will load the data from a given URL.

##### Direct Upload

Students can directly upload data files to their JupyterHub account. This method can get messy if notebooks expect the data to be stored at a certain filepath and students upload the files to a different location. Therefore, we recommend using the other methods listed on this page.

### Larger Datasets \(tens of MBs to several GBs\)

Our current recommendation is to keep the file size of the datasets below 100 GB. We recommend the following approaches to all instructors/students who plan to use large datasets for their teaching/learning plans.

#### The Shared directory (Credits: 2i2c)

##### shared

The shared folder allows read only access to the data stored for all users. You can read dataset from the shared folder while no write operations can be performed.

Create a [Github Issue](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=type%3A+enhancement&template=featurerequest.md) if you want your data to be saved in shared folder on JupyterHub directly. Notebooks stored on JupyterHub will be able to access this data.

##### shared-readwrite

shared-readwrite directory is accessible only for **administrators**. This directory allows admins read and write access to the stored data. Any data stored in the shared-readwrite appears in the shared folder for all users. 

Instructors using Stat 159 and Biology hubs use the shared directories extensively.

##### SyncThing

[SyncThing](https://syncthing.net/) is an application that allows users to share their files/folders with their collaborators through a dropox like functionality. You can store all your data in the SyncThing folder and share it with your collaborators. They can read data from the application into their Jupyter notebooks. Refer to this [documentation](https://ds-modules.github.io/curriculum-guide/workflow/use-realtimefilesharing.html) that explains the approach to share files via SyncThing.

##### Outside Hosts

You can store the data on an online host such as Box, Google Drive, or even GitHub. The `datascience` package contains a [read\_table\(\)](http://data8.org/datascience/_autosummary/datascience.tables.Table.read_table.html#datascience.tables.Table.read_table%29\) function for the [Tables](http://data8.org/datascience/tables.html%29\) data structure. This function will load the data from a given URL.