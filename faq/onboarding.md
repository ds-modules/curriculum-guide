# Get yourself onboarded to DataHub

**I am instructor planning to teach using Datahub. What should I know prior to the start of the semester?**


##### General Updates

**Proactive Support Requests:** Please submit support requests for software changes and resource allocations before instruction begins. This helps us to ensure that your requests can be accommodated and will not disrupt other course environments. Ideal time frames to make requests are either **before the start or during the first two weeks of the semester**. We recommend this timeline to ensure that we make minimal changes to the hub infrastructure when the courses are ongoing.

**Assignment Deadlines:** Please try to schedule assignments during regular working hours so that infrastructure staff can troubleshoot hubs if something goes wrong.

**Test Assignments in Advance:** Please try to test assignments and notebooks on the hub before giving them to students. This will allow time for the infra team to fix any issues you discover.

**Export to PDF Using WebPDF:** We recommend using the “Save and Export Notebook as -> WebPDF” option to convert Jupyter notebooks to PDF. We have resolved the image rendering issues previously encountered with this method and are hoping for a smoother conversion process. For more details on PDF conversion, please refer to the [documentation](https://ds-modules.github.io/curriculum-guide/workflow/download_notebook_as_pdf.html).

**Using Language Models in Assignments:** If you plan to incorporate language models into your assignments then please schedule a consultation with the infra team before releasing the assignments to students. For more details, please refer to the [documentation](https://ds-modules.github.io/curriculum-guide/technology/using-ai-llm.html).

**Datahub Link Generator:** A Berkeley specific fork of nbgitpuller browser extension called [“Datahub Link Generator”](https://chromewebstore.google.com/detail/datahub-link-generator/ijbgangngghdanhcnaliiobbiffocahf?hl=en) has been developed with few additional features. Please uninstall the old extension and reinstall the [latest version](https://chromewebstore.google.com/detail/datahub-link-generator/ijbgangngghdanhcnaliiobbiffocahf?hl=en) in Chrome so that you can get the recent updates and support. We encourage you to review this [documentation](https://ds-modules.github.io/curriculum-guide/workflow/distributing-notebooks.html#datahub-link-generator-chrome-extension) which provides detailed steps to generate assignment links through the new extension.

**Backup Students' Data:** We recommend that you inform students to back up their data (notebooks and datasets) on their local devices before the end of the semester. We have prepared [download instructions](https://ds-modules.github.io/curriculum-guide/workflow/download-archive.html) on how students can retrieve all of their archived files.  We receive a lot of student requests to retrieve their files after the completion of the semester. Any upfront communication from your end about backing up their files will hopefully ease the workload for us.

**Otter Grader Upgrade:** If you are interested in moving to the latest versions of otter-grader then please reach out to sean.smorris@berkeley.edu and ericvd@berkeley.edu.

##### DataHub - Support Overview 

**GitHub Issues:** The best way for instructional staff to request help with the DataHub is through filing an issue using the [GitHub templates](https://github.com/berkeley-dsep-infra/datahub/issues/new/choose).

**Slack Channel:** If you have anything you'd like to discuss with w/the infra team, please join the Slack channel. Access [uctech.slack.com](http://uctech.slack.com/) (anyone with a berkeley.edu account can get in) and join the #ucb-datahubs channel to interact with the infra team. 

**Datahub Service Lead:** In addition, you can reach out to Balaji Alwar <balajialwar@berkeley.edu> directly if there are time-sensitive issues.

##### Datahub - Common Requests 
**Packages:** Please test your assignments for hub compatibility before the start of the semester. Check whether all the needed Python/R packages and their required versions are installed. If not, please use the [package request template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=felder%2Cbalajialg&labels=package-request&template=package_request.yml&title=Request+python+package+X+for+class+Y) to raise a request to the infra team.  The Infra team requires at least 2 business days for a turnaround on support requests such as this.

**Elevated Privilege Access:** You can use this [GitHub template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=balajialg&labels=support&template=admin_request.yml) to request [elevated privileges](https://ds-modules.github.io/curriculum-guide/faq/admin.html?highlight=admin) for course staff to troubleshoot student servers in the requested hub. 

**Big Assignments / High Use times:** You can share the important date(s)/time(s) for workshops/exams/assignments etc. when you expect the resource requirement to be greater than usual. We will review your request and get back to you directly about the feasibility of increasing resources. You can provide us with all the relevant information using the [calendar event scheduling template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=felder%2Cbalajialg&labels=support&template=resourcescheduler.yml&title=Increase+compute+resources+for+Course+XXX+between+specific+date%28s%29%2Ftime%28s%29).

##### Other Updates

**a11y Documentation:** For further insights into improving the accessibility of the Jupyter Notebook/Lab experience for students, please review this [documentation](https://ds-modules.github.io/curriculum-guide/workflow/accessibility.html?highlight=accessibility) that provides a few tips for improving the accessibility of the notebooks.

**JupyterLab a11y Checker:**  Please check out the [JupyterLab a11y-checker extension](https://pypi.org/project/jupyterlab-a11y-checker/) that performs multiple accessibility checks on Jupyter notebook/Lab cells containing images and headings. It  does the following, a) Verifies the presence of alt-text for images, ensuring that visually impaired users can understand their content, b) Calculates the colour contrast ratio to ensure readability for low-vision users and c) Evaluates the heading structure to align with WCAG standards, ensuring that headers (h1, h2, etc.) are appropriately structured for optimal accessibility.

Finally, provide us with any feedback that will help us improve our hub operations. We want to ensure that you have a smooth experience teaching this semester.

**How can I learn more about Datahub to onboard myself?**

- If you are new to Datahub and want to know more, checkout [here](https://datahub.berkeley.edu/hub/login?next=%2Fhub%2F). 

- If you are interested in learning more about the configuration of various Berkeley hubs, you can checkout [UC Berkeley's JupyterHubs documentation](https://docs.datahub.berkeley.edu/en/latest/).

- If you want to set up a hub infrastructure at your end and are interested in learning more about the technical details, use this [Zero to JupyterHub with Kubernetes documentation](https://zero-to-jupyterhub.readthedocs.io/en/latest/).

**What languages are supported by the hub?**

Datahub primarily supports three languages - **Python, R and, Julia**. However, We also support other languages on a case-to-case basis. If you have a unique requirement for using a different programming language as part of your hub, Share your exact requirement over an email to [Eric Van Dusen](mailto:ericvd@berkeley.edu)/[Balaji Alwar](mailto:balajialwar@berkeley.edu) or raise a Github [issue](https://github.com/berkeley-dsep-infra/datahub/issues/new/choose).

**How many hubs across the campus exist? Which courses use them extensively?**

We have 15+ hubs which cater to the diverse needs of the campus audience. We have the [vanilla DataHub](https://datahub.berkeley.edu/), which serves multiple departments/courses across the campus. We also have separate hubs for courses such as Data 8, Data 100, Public health, etc., serving the instructional needs. You can learn more about some of the hubs deployed through this [link](https://docs.datahub.berkeley.edu/en/latest/users/hubs.html).

**What is the default Memory/CPU requirement for every hub?**

[DataHub](https://datahub.berkeley.edu/) has a memory of 1 GB, which should meet the teaching/research needs of most of our users. If you are interested to know more about the memory consumption in your instance, Please follow the steps below,

- Look at the top right corner of your Python/R notebook for the term memory. It will highlight the amount of memory you had consumed against the total memory available for your server. 
- If your consumed memory is greater than the available memory for your instance then your server will crash resulting in you either optimizing your workflow to be less compute intensive or requesting additional RAM,

```{figure} ../images/memory.png
:width: 500px
:align: center
:name: Available Memory

Here is where you can find the memory related details!
```
Please contact us if your course/research has more complex computation requiring increased capacity.

**What are the different services offered?**

We offer UI for Classic Jupyter Notebook, RStudio and JupyterLab across different hubs. You can learn more about the varied services offered through this jupyterhubs services [documentation](https://docs.datahub.berkeley.edu/en/latest/users/services.html).


**What is the process to raise Github issues? How can I track the raised issues?**

If you want to raise a bug, you can use this [link](https://github.com/berkeley-dsep-infra/datahub/issues/new/choose) to submit your issues.

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

**Share New Enhancement:** If you envision a new feature/documentation that would help your existing workflow, please use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=type%3A+enhancement&template=featurerequest.md) to submit a request.

**Request Package Addition/Change:** If you want to install new packages in R/Python/Julia as part of your hub, please raise a request using this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=datahub-package-addition---change-request.md&title=Request+python+package+X+for+class+Y).

**Request for RAM/CPU:** If you want to increase/decrease RAM for a specific hub then please use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=higher-resources.md&title=Request+more+RAM+for+class+X) to make the request.

**Request Admin Access:** If you want members of your teaching team to have admin access then please use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=admin_request.yml) to make this request.

**Retrieve User Data:** If you want to request data stored as part of your hub instance, then please do use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=data_archival_request.yml) to raise a request

```{note}
If these templates are not exhaustive enough to cover the type of issue you are raising, you can use this [generic template](https://github.com/berkeley-dsep-infra/datahub/issues/new) to raise your issue.
```

**As an instructor what do I need to do to set up the hub for my course?**

Honestly, nothing! You are free to use the Datahub starting today. 

```{note}
We expect that all course members log in using their UC Berkeley email id. We also expect that you are using [Datahub Link Generator](https://chromewebstore.google.com/detail/datahub-link-a/ijbgangngghdanhcnaliiobbiffocahf?hl=en) to distribute materials to your class. We can also help with setting up the links. 
```

**What instructions should I share with students at the start of the semester**
Please ask your students,

- To download and backup their files at the end of semester.
- To refrain from installing python packages via `pip install --user`. Incase, if they install packages this way it may cause issues with launching their Jupyterhub servers. Best way to avoid this scenario is by installing packages by requesting them via [issue template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=felder%2Cbalajialg%2Cshaneknapp&labels=package-request&projects=&template=package_request.yml&title=Request+python+package+X+for+class+Y)

**What if I have a student outside UC Berkeley?**

We can’t allow non UC Berkeley users as our authentication system only allows users with UC Berkeley email id. For such users, there are couple of options we recommend below, 

- Use the [Calnet Sponsored Guests](https://calnetweb.berkeley.edu/calnet-departments/calnet-sponsored-guests) option to get temporary access to bcourses which will allow you to access the Datahub service.
- Use [Binder](https://mybinder.org/) or [Jupyterlite](https://jupyterlite.readthedocs.io/en/stable/) services to solve for the immediate needs.

**How do my students download their submissions as a PDF?**
We recommend that you use the following options,
 
- **For Jupyter Notebooks:** Select File -> Download as -> WebPDF to download the PDF version of your notebook. 
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

**How do I get access to elevated privileges if I am not able to publish the bcourses site?**

As a policy, we provide elevated privileges to users **only** through their bcourses affiliation. It makes it easy for us to ensure that the right stakeholders have the elevated privileges for a particular course. If you are not using bcourses site for your course and worry that it might be confusing for your students,please create a banner in your bcourses site highlighing that you are not using bcourses for your course work. If you need more input, please contact the support team.  
