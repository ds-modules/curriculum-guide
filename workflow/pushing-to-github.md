# Pushing to GitHub

# Using the Web Interface

You can perform many actions such as uploads and downloads directly through GitHub's web interface directly, without having to use the command line interface. Here are some directions on how to upload assignments to GitHub. If you did your development on JupyterHub, \[download the notebook\]\([https://github.com/data-8/connector-instructors/wiki/Creating-Notebooks\#download\](https://github.com/data-8/connector-instructors/wiki/Creating-Notebooks#download%29\) onto your computer. Then, go to your connector's GitHub repository and click \`Upload Files\` on the right side.

![](https://cloud.githubusercontent.com/assets/8205702/23319695/89fa6484-fa8c-11e6-9d36-6b6782e2c383.png)

You can drag and drop your desired files onto the page. Then, write a short sentence describing the files you're adding. This short sentence is called a commit message.

![](https://cloud.githubusercontent.com/assets/8205702/23319707/9a4d26b4-fa8c-11e6-91e7-72eeef8bce86.png)

You will then see an option to select the branch for your changes. The default for most repositories will be the \`master\` branch. If you are a Git beginner, you can stick to the default and add your changes to the \`master\` branch. If you are a more advanced Git user and want to use different branches, you may want to select the option to create a new branch. Please see the additional GitHub resources on this page to learn more about branching.

![](https://cloud.githubusercontent.com/assets/8205702/23319711/9cf7b2da-fa8c-11e6-818e-c231b29a5040.png)

Once you've gone through the above steps, you can save your changes. A set of changes in Git is called a commit.

## ![](https://cloud.githubusercontent.com/assets/8205702/23319717/9f1fb81e-fa8c-11e6-86ae-074f2c11e9f5.png)

## Using the Command Line

GitHub can also be used via the command line. You can store your connector's Git repository locally and use a local terminal application to access the command line. You can also store the repository on \[datahub.berkeley.edu\]\([http://datahub.berkeley.edu\](http://datahub.berkeley.edu%29\) and use the terminal that is present on the JupyterHub site. The instructions below are tailored towards command line use over JupyterHub, but the commands listed can be run on a local terminal as well.

You can access the terminal on JupyterHub by clicking on the \`New\` dropdown, and then clicking on \`Terminal\`.

![](https://cloud.githubusercontent.com/assets/8205702/23319236/9ca1a018-fa8a-11e6-8c3d-e5d084317ccc.png)

You will then see a terminal page in the browser.

![](https://cloud.githubusercontent.com/assets/8205702/23321085/a981a654-fa92-11e6-98e2-f64bf92600bc.png)

In order to push to your connector's repository, you must have the repository downloaded \(aka cloned\). If you have not yet cloned the repository, type the below command into the terminal. The \`&lt;repo\_name&gt;\` is the name of the repository for your connector. The repository names are listed at [https://github.com/data-8](https://github.com/data-8). Once you run the below command, you will see a folder for your repository in your home directory on JupyterHub. \*\*You do not have to repeat this step again.\*\*

```
    git clone https://github.com/data-8/&lt;repo\_name&gt;
```

For example, if your repository is called \`health-connector\`, you'd type:

```
    git clone https://github.com/data-8/health-connector
```

After this step, you should be able to see your connector's folder at \[[https://datahub.berkeley.edu\]\(https://datahub.berkeley.edu\](https://datahub.berkeley.edu]%28https://datahub.berkeley.edu%29%29. Create, upload, or move content %28Notebooks, datasets, etc.\) into the folder. For more information on creating Notebooks, see \[this page\]\([https://github.com/data-8/connector-instructors/wiki/Creating-Notebooks\](https://github.com/data-8/connector-instructors/wiki/Creating-Notebooks%29\). For more information on storing datasets, see \[this page\]\([https://github.com/data-8/connector-instructors/wiki/Storing-Datasets\](https://github.com/data-8/connector-instructors/wiki/Storing-Datasets%29\). Once you have your content in the newly created connector repository folder, you can follow the steps below on the terminal to push to GitHub.

```
    cd ~/&lt;repo\_name&gt;

    git status
```

You should see something that lists the files you've changed or added. If your files don't show up, ensure that they are in your repo's folder.

```
    git add -A

    git commit -m "Update"

    git push origin master
```

If the push is successful, you should be able to go \[GitHub\]\([https://github.com/data-8\](https://github.com/data-8%29\) and see the newly uploaded file in the connector repo. If you run into something that looks the below error, contact us on \[Piazza\]\([https://piazza.com/berkeley/other/cs97\](https://piazza.com/berkeley/other/cs97%29\) and we will make sure you have the permissions needed.

```
    ERROR: Permission to data-8/some-connector.git denied
```

Here are the above commands, consolidated. This workflow is intended for Git beginners. Git offers many additional features that are not demonstrated in these steps.

```
    git clone https://github.com/data-8/&lt;repo\_name&gt;

    cd ~/&lt;repo\_name&gt;

    git status

    git add -A

    git commit -m "Update"

    git push origin master
```

## Additional Resources

**Web Interface**

* [Managing Files](https://help.github.com/categories/managing-files-in-a-repository/\) - contains information under the "Managing Files on GitHub" section on how to perform many basic file operations using the GitHub web interface.

* [Hello World Exercise](https://guides.github.com/activities/hello-world/\)[ ](https://guides.github.com/activities/hello-world/%29\)- a short exercise that walks you through additional GitHub features such as branches and pull requests.

**Command Line**

* [Atlassian Tutorials](https://www.atlassian.com/git/tutorials\) - tutorials for different levels of Git Users.

**Desktop GUI**

* [Desktop GUI site](https://desktop.github.com/\) - information on using a GitHub desktop GUI.



