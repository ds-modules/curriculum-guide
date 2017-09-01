# Distributing Notebooks

We recommend using interact links to distribute notebooks to students. These links allow students to obtain all files and folders needed for an assignment with just one click. Students do not need to download files and the upload them back to their JupyterHub account.

If you do not wish to use interact links, you can distribute assignments through bCourses as well. In this case, after you have uploaded the files to bCourses, students will need to download them and then upload them to their own JupyterHub accounts.

## Interact Links

### What are interact links?

Interact links simplify the assignment distribution process. Rather than downloading files from an external source and then uploading to their personal JupyterHub accounts, users can obtain all files for a given assignment with just one click. When a user clicks on an interact link for a particular assignment, all files for the assignment will show up in the user's personal JupyterHub account.

These links can be used with any content stored on GitHub in a public repository. Interact links can be generated for an entire repository, or a particular file or folder. 

### How do the links work?

Interact links are running a series of git commands from the user's JupyterHub account when they are clicked. This is why interact links must be used with content on GitHub. They cannot be used to pull arbitrary files from sources other than GitHub. 

Here is an interact link with the various components highlighted in different colors. The grey portions of the link are needed for formatting and will remain the same for each links. The colored portions will be different for each link. If you are new to GitHub you may want to familiarize yourself with the basics \(repositories, branches, etc.\) to better understand each component.

### ![](/assets/interact-link.png)**Restrictions**

To use an interact link, files must be stored in a public GitHub repo. Interact links will not work with private repositories.

### **Interact Link Generator**

Interact links can be manually created in the format shown above, or can be automatically generated using [this](https://url-to-interact.herokuapp.com\) tool. The interact link generator tool allows users to specify a JupyterHub URL and GitHub url as inputs. The tool will generate an interact link for the specified GitHub content and JupyterHub.

For example, to pull [this](https://github.com/data-8/mcb-88-connector/tree/gh-pages/exercises/lab5) folder into a JupyterHub account on datahub.berkeley.edu, select "datahub.berkeley.edu" as the desired hub, paste the GitHub url "[https://github.com/data-8/mcb-88-connector/tree/gh-pages/exercises/lab5](https://github.com/data-8/mcb-88-connector/tree/gh-pages/exercises/lab5)" into the generator, and hit the convert button. The output should be "[https://datahub.berkeley.edu/user-redirect/interact?account=data-8&repo=mcb-88-connector&branch=gh-pages&path=exercises/lab5](https://datahub.berkeley.edu/user-redirect/interact?account=data-8&repo=mcb-88-connector&branch=gh-pages&path=exercises/lab5)". This link will copy the desired folder into JupyterHub.

