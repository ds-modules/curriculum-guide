# Pedagogy and Technology

The technology used in the Data Science Education Program \(DSEP\) was chosen to support the needs and goals of the program. In order to make the courses accessible to students of all majors requires, we wanted to use technology that was simple but powerful. We did not want students to deal with the frustrations of setting up and maintaining a development environment, which are often experienced in introductory computing courses. In Data 8, students do not have to waste any time on installation or setup, which means they are able to write and run code from the start.

## JupyterHub and Notebooks

Jupyter Notebooks and JupyterHub are the tools that enable this student experience. You may have experience using Jupyter Notebooks on your own computer. Students in DSEP run their notebooks entirely in the cloud, on a JupyterHub. Python and common packages are preinstalled on each student's account, which is created when the student first logs in with an approved email. A lot of work goes into the maintenance of the infrastructure and many students, TAs, and staff members are regularly monitoring and fixing issues that come up.

## `datascience` package

In addition to the computing infrastructure, another piece of the technology is the `datascience` package. While traditional libraries such as `pandas` and `matplotlib` are powerful, they are also quite complicated, and the verbose code and documentation can intimidate those who are new to programming. The `datascience` Python package was written for use in Berkeley’s Data Science courses and aims to provide a simple but powerful set of tools for introductory students. The package contains useful functionality for investigating and graphically displaying data. One key component of the `datascience` package is the `Tables` abstraction, which is similar to a Pandas dataframe. The package also contains useful functionality for drawing maps and plotting.

