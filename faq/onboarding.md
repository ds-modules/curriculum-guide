# Get yourself onboarded to DataHub

```
**I am instructor planning to teach using Datahub. What should I know prior to the start of the semester?**

Dear Instructor, Datahub team is available to support you through this process. Sharing few onboarding tips that would make it easy for you to get familiar with Datahub and interact with the support team.

- **Github Issues:** The best way to request help with the Datahub is handled through filing an issue on the github page for the datahub deployment: https://github.com/berkeley-dsep-infra/datahub/issues
- **Slack Channel:** For urgent troubleshooting, you or your course staff can also use uctech.slack.com (anyone with a berkeley.edu account can get in) and join the #ucb-datahubs channel to touch base with the infra team. 
- **Documentation:** You can also refer to the FAQ section of this support documentation where we regularly update solutions to some of the reported issues.
 - **Packages:** Check whether all the needed Python/R packages along with their required versions are installed in the instructional hubs you use for teaching. If certain packages are not present, please use the following [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=felder%2Cbalajialg&labels=package-request&template=package_request.yml&title=Request+python+package+X+for+class+Y) to make a request to the support team.  
- **Elevated Privileges:** Do you want your instructional staff to troubleshoot student servers when they have issues. You can get elevated privileges which allows for viewing and accessing student servers in DataHub. If you need to access student servers, You can use this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=balajialg&labels=support&template=admin_request.yml) to make the request for the requested hub.
- **Big Assignments / High Usage times:** You can share the important date(s)/time(s) for workshops/exams/assignments etc. in your course the compute requirement is greater than regular usage during this semester. You can provide us with the required information using this [template](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=felder%2Cbalajialg&labels=support&template=resourcescheduler.yml&title=Increase+compute+resources+for+Course+XXX+between+specific+date%28s%29%2Ftime%28s%29).
- **Newsletter:** Are you interested to learn about some of the latest infrastructure changes, case studies of faculty doing interesting work, and scheduled workshops related to Datahub and other tools part of Berkeley Data Science Teaching Stack? If yes, Check our [newsletter](https://ucberkeleydatahub.substack.com/p/january-edition-of-berkeley-datahub) and subscribe to it if you think the information shared is useful! Some new things to know about are,
- **Datahub Link Generator Plugin:** There is a [plugin in the Google Chrome store](https://chromewebstore.google.com/detail/datahub-link-generator/ijbgangngghdanhcnaliiobbiffocahf?hl=en) which helps with generating distributable links from Github. 

Finally, provide us with any [feedback](https://github.com/berkeley-dsep-infra/datahub/issues/new) that will help us improve our hub operations. We want to ensure that you have a smooth experience teaching this semester. 

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
