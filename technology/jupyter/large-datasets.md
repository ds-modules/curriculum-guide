# Storing Datasets

### Datasets under 200MB

##### GitHub

Datasets and the corresponding Jupyter Notebook can be stored in a folder on GitHub. You can then create an interact link for the entire folder. When students click this link, the entire folder will appear on their JupyterHub account.

##### Outside Hosts

You can store the data on an online host such as Box, Google Drive, or even GitHub. The `datascience` package contains a [read\_table\(\)](http://data8.org/datascience/_autosummary/datascience.tables.Table.read_table.html#datascience.tables.Table.read_table%29\) function for the [Tables](http://data8.org/datascience/tables.html%29\) data structure. This function will load the data from a given URL.

##### Direct Upload

Students can directly upload data files to their JupyterHub account. This method can get messy if notebooks expect the data to be stored at a certain filepath and students upload the files to a different location. Therefore, we recommend using the other methods listed on this page.

### Datasets over 200MB

##### Shared Copy on JupyterHub

Contact us on [Piazza](https://piazza.com/berkeley/other/cs97\) if you want your data to be saved in shared folder on JupyterHub directly. Notebooks stored on JupyterHub will be able to access this data.

