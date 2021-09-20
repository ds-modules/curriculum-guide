# Onboarding new users to the Hub

```{note}
New to Datahub? Interested to learn more about the services offered by the hub? If yes, refer below!
```

**How can I learn more about Datahub to onboard myself?**

- If you are new to Datahub and want to know more, refer [here](https://datahub.berkeley.edu/hub/login?next=%2Fhub%2F). 

- If you are interested in learning more about the configuration of various Berkeley hubs, you can refer to [UC Berkeley's JupyterHubs documentation](https://docs.datahub.berkeley.edu/en/latest/).

- If you want to set up a hub infrastructure at your end and are interested in learning more about the technical details, use this [Zero to JupyterHub with Kubernetes documentation](https://zero-to-jupyterhub.readthedocs.io/en/latest/).

**What languages are supported by the hub?**

Datahub primarily supports three languages - **Python, R and, Julia**. However, We can also support other languages on a case-to-case basis. If you have a unique requirement for using a different programming language as part of your hub, Share your exact requirement over an email to [Eric Van Dusen](mailto:ericvd@berkeley.edu)/[Balaji Alwar](mailto:balajialwar@berkeley.edu) or raise a Github [issue](https://github.com/berkeley-dsep-infra/datahub/issues/new/choose).

**How many hubs across the campus exist? Which courses use them extensively?**

We have 15+ hubs that cater to the diverse needs of the campus audience. We have the main Datahub, which serves multiple departments/courses across the campus. In addition, We have separate hubs for courses such as Data 8, Data 100, Public health, etc., serving the teaching team's and enrolled students needs. You can learn more about some of the hubs deployed through this [link](https://docs.datahub.berkeley.edu/en/latest/users/hubs.html).

**What is the default Memory/CPU requirement for every hub?**

Datahub has a memory limit of 1 GB of RAM, which should meet the teaching/research needs of most of our users. If you are interested to know more about the memory consumption in your instance, Please use the following steps,

- Look at the top right corner of your Python/R notebook for the term memory. It will highlight the amount of memory you had consumed by the amount of memory provided to your instance. 
- If your consumed memory is greater than the available memory for your instance, You may require an increase in RAM,

```{figure} ../images/memory.png
:width: 500px
:align: center
:name: Available Memory

Here is where you can find the memory related details!
```
Please contact us if your course/research has more complex computation requiring increased capacity.

**What are the different services offered as part of the Datahub?**

We offer UI for Classic Jupyter Notebook, RStudio and JupyterLab across different hubs. You can learn more about the varied services offered through this jupyterhubs services [documentation](https://docs.datahub.berkeley.edu/en/latest/users/services.html).

**What are the packages pre-installed for every hub?**

Package installation varies across the different hubs. We ensure that basic python packages such as numPy, pandas, scikit-learn, matplotlib, etc., are installed across all the Jupyter hubs. Our R hubs also support shiny, dplyr, tidyR, RSQLlite, etc. However, you can customize the packages for the hubs by requesting them using this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=datahub-package-addition---change-request.md&title=Request+python+package+X+for+class+Y).

If you want to check the list of packages installed, 

- You can use the below option for Python,
 
```python
!pip list
```
- You can use the below option for R,

```
installed.packages()
```
- You can check the packages installed in Julia by accessing the [Julia Hub](http://julia.datahub.berkeley.edu/)

```{note}
Here is the [list](https://github.com/berkeley-dsep-infra/datahub/blob/staging/deployments/datahub/images/default/requirements.txt) of Python packages installed in Datahub. Here is the [list](https://github.com/berkeley-dsep-infra/datahub/blob/staging/deployments/datahub/images/default/install.R) of R packages installed in Datahub.
```


**What is the process to raise Github issues? How can I track the raised issues?**

If you want to raise a bug, you can use this [link](https://github.com/berkeley-dsep-infra/datahub/issues/new/choose) to submit your issues. You can also use post messages to our [Piazza channel](https://piazza.com/class/ksqmnrrhvcl11f) if you require real time troubleshooting!

**When do I receive a response when an issue gets raised?**

```{note}
Please refer to the below Service Level Agreement (SLA) for varied requests. Time for this SLA will start from the time when we have complete information regarding your request,
```

- SLA for package installation: "Acknowledgement within two working days."
- SLA for RAM increase: "Acknowledgement within two working days."
- SLA for admin access: "Request completed within two working days."
- SLA for data archival request: "Request completed within three working days."

**Are there existing templates for submitting requests to the infrastructure team?**

We have categorized common requests we get from our users into templates that you can repurpose to make your request. You can refer to the following templates catering to varied scenarios,

**Raise Bugs:** If you found a bug in the workflow, Please use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=bug&template=bug_report.yml) to raise an issue.

**Share a New Enhancement:** If you envision a new feature/documentation that would help your existing workflow, please use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=type%3A+enhancement&template=featurerequest.md) to submit a request.

**Request Package Addition/Change:** If you want to install new packages in R/Python/Julia as part of your hub, please raise a request using this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=datahub-package-addition---change-request.md&title=Request+python+package+X+for+class+Y).

**Request for RAM/CPU:** If you want to increase/decrease RAM for a specific hub then please use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=higher-resources.md&title=Request+more+RAM+for+class+X) to make the request.

**Request Admin Access:** If you want members of your teaching team to have admin access then please use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=admin_request.yml) to make this request.

**Request to recover hub data:** If you want to request data stored as part of your hub instance, then please do use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=data_archival_request.yml) to raise a request

```{note}
If these templates are not exhaustive enough to cover the type of issue you are raising, you can use this [generic template](https://github.com/berkeley-dsep-infra/datahub/issues/new) to raise your issue.
```

**As an instructor what do I need to do to set up the hub for my course?**

Honestly, nothing! You are free to use the Datahub starting today. 

```{note}
We expect that all course members log in using their UC Berkeley email id. We also expect that you are using [nbgitpuller service](https://jupyterhub.github.io/nbgitpuller/link) to distribute materials to your class. We can help you set up the links so that you can distribute through your course website. 
```

**What if I have a student outside UC Berkeley?**

We can’t allow non UC Berkeley users as our authentication system only allows users with UC Berkeley email id. For such users, there are couple of options we recommend below, 

- Use the [Calnet Sponsored Guests](https://calnetweb.berkeley.edu/calnet-departments/calnet-sponsored-guests) option to get temporary access to bcourses which will allow you to access the Datahub service.
- Use [Binder service](https://mybinder.org/) to solve for the immediate needs.

**How do my students download their submissions as a PDF?**
We recommend that you use the following options,
 
- **For Jupyter Notebooks:** Select File -> Download as -> PDF via HTML(.pdf) to get the PDF version of your notebook. 
```{figure} ../images/downloadhtml.PNG
:width: 500px
:align: center
:name: Downloading notebook as a PDF 
Here is where you can find the option to download the Python notebook as a PDF!
```
- **For R files:** Select File -> Knit Document -> Select the target folder -> Select the Output Format as PDF to save the PDF version of the file
 ```{figure} ../images/knitting.PNG
:width: 500px
:align: center
:name: Downloading R notebook as a PDF
Here is where you can find the option to download the R file!
```
```{figure} ../images/knittingpdf.PNG
:width: 500px
:align: center
:name: Downloading notebook as a PDF
Here is where you can find the option to specify the download format as PDF!
```
