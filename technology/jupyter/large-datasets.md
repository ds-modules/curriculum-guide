# Storing Datasets

A few methods of storing datasets are outlined below. The choice of method depends on your preference and the size of the dataset. Keep in mind, regardless of the size of your dataset, each account on DataHub is provided with ~1GB RAM, so this will limit the amount of data that you can read in at any time. If you want to temporarily increase this limit on RAM, please raise a [github issue](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=support&template=higher-resources.md&title=Request+more+RAM+for+class+X).

### Small Datasets \(a few MBs\)

##### GitHub

Datasets and the corresponding Jupyter Notebook can be stored in a folder on GitHub. You can then create a nbgitpuller link for the entire folder. When students click this link, the entire folder will appear on their DataHub account.

##### Outside Hosts

You can store the data on an online host such as Box, Google Drive, or even GitHub.

##### Direct Upload

Students can directly upload data files to their DataHub account. This method can get messy if notebooks expect the data to be stored at a certain filepath and students upload the files to a different location. Therefore, we recommend using the other methods listed on this page.

### Larger Datasets \(tens of MBs to several GBs\)

Our current recommendation is to keep the file size of the datasets below 100 MB. We recommend the following approaches to all instructors/students who plan to use large datasets for their teaching/learning plans.

#### Shared directory

In scenarios where you have large datasets or commonly used libraries, a shared directory can serve as a centralized location for these resources. This prevents the need for duplicating files across multiple user spaces, saving disk space and bandwidth.

**Shared Directory**: The shared folder allows read only access to the students enrolled in your course. Students can read the dataset from the shared folder while no write operations can be performed. The shared directories will be mounted to `/home/jovyan` user path.

```{note}
By default, students cannot write to shared directories. While configuration can be modified to allow students to write to the shared directories, it is generally not recommended. Allowing write access to a shared directory can lead to students accidentally overwriting each other’s work, especially if they’re working simultaneously. Typically, instructors prefer that students save their work in their home directories and then upload the necessary files to a centralized drive or repository. Having said that, We can enable read access for students if you as an instructor is okay with the risks involved.
```

**Shared-ReadWrite Directory** As an instructor, you'll have both read and write access to a "shared-readwrite" directory. You can upload datasets there, and they will automatically be updated in the "shared" directory, which is accessible to all students with read-only permissions. 

```{note}
This setup streamlines the workflow: you upload datasets to the "shared-readwrite" directory, and students can immediately access them in the "shared" directory and read it.
```

Create a [Github Issue](https://github.com/berkeley-dsep-infra/datahub/issues/new?assignees=&labels=type%3A+enhancement&template=featurerequest.md) if you want shared directories enabled for your course. You need to provide the bcourses id for your course and the DataHub URL so that the shared directories appear on the hub you use with appropriate permissions for the folks enrolled in your course roster in bcourses.

Eg:`compss-214a-readwrite` and `compss-214a` are the shared-readwrite and shared directories for the COMPSS-214A course.

```{warning}
- Communicate to your students that those enrolled in your previous course offering lose access to the shared directories at the end of the semester. 
- Please verify that neither you nor your teaching team members are enrolled in multiple roles (e.g., both Teacher and TA) on your course's bCourses site. Being assigned multiple roles may cause errors during hub spawning, as the system attempts to mount multiple shared read-write directories associated with different group roles (e.g., Teacher and TA).
```

##### SyncThing

[SyncThing](https://syncthing.net/) is an application that allows users to share their files/folders with their collaborators through a dropox like functionality. You can store all your data in the SyncThing folder and share it with your collaborators. They can read data from the application into their Jupyter notebooks. Refer to this [documentation](https://ds-modules.github.io/curriculum-guide/workflow/use-realtimefilesharing.html) that explains the approach to share files via SyncThing.

##### Outside Hosts

You can store the data on an online host such as Box, Google Drive, or even GitHub. The `datascience` package contains a [read\_table\(\)](http://data8.org/datascience/_autosummary/datascience.tables.Table.read_table.html#datascience.tables.Table.read_table%29\) function for the [Tables](http://data8.org/datascience/tables.html%29\) data structure. This function will load the data from a given URL.