# Distributing Notebooks

We recommend using interact links to distribute notebooks to students. Interact links are described in detail below. If you do not wish to use interact links, you can distribute assignments through bCourses as well. In this case, after you have uploaded the files to bCourses, students will need to download them and then upload them to their own JupyterHub accounts.

### The Steps

Here are the basic steps you will need to go through to distribute notebooks and other files. Thes

1. Add all files for an assignment into a folder
2. Upload folder to a public GitHub repository
3. Generate an interact link for the folder using the [interact link generator](https://url-to-interact.herokuapp.com)
4. Distribute the link to students through some web page

---

### What are interact links?

Interact links simplify the assignment distribution process. Rather than downloading files from an external source and then uploading to their personal JupyterHub accounts, users can obtain all files for a given assignment with just one click. When a user clicks on an interact link for a particular assignment, all files for the assignment will show up in the user's personal JupyterHub account.

These links can be used with any content stored on GitHub in a public repository. Interact links can be generated for an entire repository, or a particular file or folder. When a link is clicked, a series of Git commands are run from the user's JupyterHub account, which is why interact links must be used with content on GitHub. They cannot be used to pull arbitrary files from sources other than GitHub.

Using these links enables users to immediately interact with publicly available content on GitHub. This is valuable for easy assignment distribution, but also in the broader context of using the open-source content that is available on GitHub. Learning Git is no longer a barrier to interacting with this content.

### How do interact links work?

Here is an interact link with the various components highlighted in different colors. The grey portions of the link are needed for formatting and will remain the same for each links. The colored portions will be different for each link. If you are new to GitHub you may want to familiarize yourself with the basics \(repositories, branches, etc.\) to better understand each component.

![](/assets/interact-link.png)The above link does the following:

* Clone the `social-networks-connector` repo from the `data-8` GitHub organization into the user's account on `datahub.berkeley.edu`
* Checkout to the `gh-pages` branch
* Redirect the user to the `lab01` folder on `datahub.berkeley.edu`. The full path of this folder on the user's JupyterHub account would be `~/social-networks-connector/lab01`.

### Restrictions

To use an interact link, files must be stored in a public GitHub repo. Interact links will not work with private repositories. Previously, content had to be stored in the `data-8` GitHub organization or in an approved account or organization. This no longer applies, interact links can be used with content stored in ANY public repository.

### **Important Note: Updated Behavior**

Previously, interact links had a slightly different behavior. They used a sparse checkout to only pull the files specified after `path`. For the above link, this would mean that only the `lab01` folder is displayed in the `social-networks-connector` folder. Any other files in the `social-networks-connector` repo would not show up in the user's JupyterHub. This is no longer the behavior. The new behavior does not use sparse checkout. For the above link, in addition to the `lab01` folder, all other contents of the `social-networks-connector` repo will show up in the user's JupyterHub account.

This new behavior means that **you should not store unfinished materials and answer keys in the same repo as published assignments**. Any interact link for a published assignment would also distribute the unfinished materials and answer keys to the students, which you probably do not want. Instead, **we recommend that you use a public repo for published assignments and a private repo for unfinished materials and answer keys**.

Here is a demo showing both the new and old behavior of interact links. To understand the difference, compare the contents of the `lab` folder in each case.

* [New behavior](http://datahub.berkeley.edu/user-redirect/interact?repo=data8assets&path=materials/sp17/lab/lab01 ) - all lab folders present at `~/data8assets/materials/sp17/lab`
* [Old behavior](http://data8.haas.berkeley.edu/user-redirect/interact?repo=data8assets&path=materials/su17/lab/lab01 ) - just `lab01` folder present at `~/data8assets/materials/su17/lab`

### **Interact Link Generator**

Interact links can be manually created in the format shown above, or can be automatically generated using [this](https://url-to-interact.herokuapp.com\) tool. The interact link generator tool allows users to specify a JupyterHub URL and GitHub url as inputs. The tool will generate an interact link for the specified GitHub content and JupyterHub.

For example, to pull [this](https://github.com/data-8/mcb-88-connector/tree/gh-pages/exercises/lab5) folder into a JupyterHub account on `datahub.berkeley.edu:`

* Select `datahub.berkeley.edu` as the desired hub
* Paste the GitHub url [https://github.com/data-8/mcb-88-connector/tree/gh-pages/exercises/lab5](https://github.com/data-8/mcb-88-connector/tree/gh-pages/exercises/lab5) into the generator
* Hit the convert button 

The output should be [https://datahub.berkeley.edu/user-redirect/interact?account=data-8&repo=mcb-88-connector&branch=gh-pages&path=exercises/lab5](https://datahub.berkeley.edu/user-redirect/interact?account=data-8&repo=mcb-88-connector&branch=gh-pages&path=exercises/lab5). This link will copy the desired folder into your JupyterHub account.

