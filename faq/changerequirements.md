# Changing existing requirements

```{note}
Interested to learn more about how to change the default requirements for your hub? If yes, read below!

```

**What should I do if I want to install more packages?**

- Use your datahub instance to install the required version of the package. Self installation of packages in your instance of hub is a temporary measure to identify dependencies. If you require a permanent solution then you need to [request](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=datahub-package-addition---change-request.md&title=Request+python+package+X+for+class+Y) us to install the required package(s) in your hub.

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

**How can I increase per-user RAM/CPU?**

We recommend instructors to adapt the materials to the 1GB requirement of the Datahub as it is convenient for most usecases. However, If you have a compelling reason to request for more RAM/CPU, use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=higher-resources.md&title=Request+more+RAM+for+class+X). Provide rationale for this upgrade as it has cost implications for the service.

There are three factors we consider as part of the requests related to increasing RAM:

- Number of students
- RAM requested
- Amount of time the resource increase is requested for.

You can request resources for all students in the class, or for a subset of students that have been placed into a [bCourses group](https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-manually-create-groups-in-a-group-set/ta-p/700). The latter might be useful for when you need to temporarily increases resources for a particular assignment.

```{list-table}
:header-rows: 1

* - Duration
  - Auto-approval (student count * RAM) threshold
* - < 1 week
  - 600 GB
* - < 1 month
  - 400 GB
* - More than 1 month
  - 200 GB
```
 Any request for more resources than the highlighted ones in the above table requires further consideration at our end.

CPU grant requests are more complex as they they are more likely to affect performance of other users on the hub. As a result, every request would require further consideration at our end.

**As an instructor, What should I do if I want to conduct a workshop? Are there any existing hubs that I could repurpose?**

Yes. We certainly do support using our hubs for workshops. For example, [D-Lab](https://dlab.berkeley.edu/) uses Datahub to run its R workshops for students regularly.

Please send an email to Eric Van Dusen (ericvd@berkeley.edu)/Balaji Alwar (balajialwar@berkeley.edu) with the specific request you have in mind. 

```{note}
We would like to know 
- Your exact need
- Memory/CPU requirement 
- Total number of participants 
- Dataset size, and 
- Language required
```

**As a researcher, What is the process to request a hub focused on research?**

Our primary motive for the hubs is to support the teaching practices of our instructors. However, if you are interested in doing core research, we recommend contacting the team at [Research IT](https://research-it.berkeley.edu/), who may support you with your specific use-case.

 ```{tip}
You might benefit from checking out their High Performance Computing Cluster [Savio](https://research-it.berkeley.edu/services-projects/high-performance-computing-savio) and [On Demand Virtual Machines](https://research-it.berkeley.edu/services-projects/aeod-virtual-machines).
```

**I am going to run a large dataset for my class. What are the steps I can take to ensure that the hub has the required compute power?**

As a rule of thumb, we recommend the following steps. If these steps are not helpful, reach out to us separately,

- Github has a file upload limit of 100 MB. Considering this, We recommend that you keep the dataset size below 100 MB. You could either create a subset of the dataset or find another dataset that fits the size limits for overcoming this constraint. 
 
 ```{tip}
Most of the issues with the dataset arise due to the programming practices used while operating the dataset, such as a lot of machine time spent reading/writing to the disk or single-threaded executions that can max the allocated CPU.
```
 
- If resizing the dataset is not feasible, Profile your system to understand the CPU/Memory consumption while operating on the dataset. Use this data to take modify your programming practices so that you are within the allocated CPU/RAM size. If you are using python, this [resource](https://docs.python.org/3/library/debug.html) will be helpful to understand your memory/CPU conusmption. If you are using R, this [resource](https://support.rstudio.com/hc/en-us/articles/218221837-Profiling-R-code-with-the-RStudio-IDE) may be helpful with profiling.


**What should I do If I want to switch from an existing hub to an R hub?**

You can directly use the [R Datahub](http://r.datahub.berkeley.edu/) dedicated to serving courses using R. If you have other specific requirements, please do reach out to us.

**When can I create a new hub?**

We generally prefer using our existing hubs for teaching your courses. Our guiding principles for allowing the creation of new hub are,

 ```{note}
- When the course has a large user base

- When there is a need for undergrad students to have admin access

- When there is a specific technical/architectural reasons

- When there is a strong institutional/strategic reason
```

**As an instructor, Can I request a custom image with different installation requirements?**

It depends on your requirements. Please send an email to [Eric Van Dusen](mailto:ericvd@berkeley.edu)/[Balaji Alwar](mailto:balajialwar@berkeley.edu) with your detailed requirement.
