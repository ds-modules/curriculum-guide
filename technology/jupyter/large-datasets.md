# Storing Datasets

## Datasets under 200MB

### GitHub

Datasets and the corresponding Jupyter Notebook can be stored in a folder on GitHub. You can then create an interact link for the entire folder. When students click this link, the entire folder will appear on their JupyterHub account.

### Outside Hosts

You can store the data on an online host such as Box, Google Drive, or even GitHub. You can then include a cell with this \[\`download\_dataset\` function\]\([https://github.com/data-8/connector-instructors/blob/gh-pages/connectortools/utils.py\](https://github.com/data-8/connector-instructors/blob/gh-pages/connectortools/utils.py%29\) or have students read the data directly via URL. The \[\`read\_table\` function\]\([http://data8.org/datascience/\_autosummary/datascience.tables.Table.read\_table.html\#datascience.tables.Table.read\_table\](http://data8.org/datascience/_autosummary/datascience.tables.Table.read_table.html#datascience.tables.Table.read_table%29\) for the \[Table\]\([http://data8.org/datascience/tables.html\](http://data8.org/datascience/tables.html%29\) data structure supports URLs.

### Direct Upload

Students can directly upload data files that you provide them onto their JupyterHub accounts. This method can get messy if notebooks expect the data to be stored at a certain filepath and students upload the files to a different location. Therefore, we recommend using the other methods listed on this page.

## Datasets over 200MB

### Shared Copy on JupyterHub

Contact us on [Piazza](https://piazza.com/berkeley/other/cs97\) if you want your data to be saved in shared folder on JupyterHub directly. Notebooks stored on JupyterHub will be able to access this data.

