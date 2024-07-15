# Welcome to the UC Berkeley Data Science Curriculum Guide!

## The Guide has Moved!

This guide is now located at [ds-modules.github.io/curriculum-guide](https://ds-modules.github.io/curriculum-guide).

### What is this guide and who is it for?

The information in the guide is primarily intended for instructors who either currently are or will be teaching a course in the UC Berkeley Data Science Education Program: either a connector course, a data-enabled course, or a course featuring a data science module. However, anyone else who wants to learn more about the program, the courses, and the technology is encouraged to look through the guide.

### Build Instructions (heavily borrowed from Shane's update in https://github.com/berkeley-dsep-infra/datahub-usage-analysis)

# Working in this repo

## SSH keys
If you've created `ssh` keys previously, please skip to the next step.

### Ubuntu/WSL2
If you're running Ubuntu, regular installation/VM or WSL2, and have NOT
previously generated SSH keys please execute the following commands:
```
ssh-keygen -t rsa -b 8192
```
For added security, you can choose to enter a passphrase during key creation.
This is optional.

### Macos
If you're using macos, and have NOT previously generated SSH keys please
execute the following commands:
```
ssh-keygen -t rsa -b 8192
```
For added security, you can choose to enter a passphrase during key creation.
This is optional.

### Windows
If you're running Windows, please install either [WSL2 native linux](https://learn.microsoft.com/en-us/windows/wsl/install) 
or [gitbash](https://www.git-scm.com/download/win).

Open a terminal, and run the following command.  WSL2 is preferred, but there
are a few additional steps required.

```
ssh-keygen -t rsa -b 8192
```
For added security, you can choose to enter a passphrase during key creation.
This is optional.

### Upload your public ssh key to GitHub
Please follow the instructions [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) 
to upload your SSH public key to GitHub.  This allows you to authenticate while
using `git` in a repo.

## Setting up your fork and clones

When you log in to your terminal, you will be in your home directory.  We
recomend creating a sub-directory named something like `src` or `repos`.  This
will help you manage any other repos you might download.

```
$ pwd
/home/username
$ mkdir repos
$ cd repos
```

Next, go to the [Curriculum Guide github repo](https://github.com/ds-modules/curriculum-guide)
and create a fork.  To do this, click on the `fork` button and then
`Create fork`.

Now clone the Curriculum Guide repo on your local device. You
can get the URL to do this by licking on the green `Code` button in the primary
[Curriculum Guide](https://github.com/berkeley-dsep-infra/curriculum-guide/)
repo (*not* your fork) and clicking on `ssh` and copying the value in the box.

Before you clone, make sure that you're in the subdirectory that will contain
this repo:
```
$ pwd
/home/username/repos
```

Now you can run the `git clone` command:
```
git clone git@github.com:ds-modules/curriculum-guide.git
```

Now `cd` in to `curriculum-guide` directory and set up your local repo
to point both at the primary repo (`upstream`) and your fork (`origin`).  After
the initial clone, `origin` will be pointing to the main repo and we'll need
to change that.

Here is an example, including output, of how to set up your remotes:
```
$ cd curriculum guide
$ git remote -v
origin	git@github.com:ds-modules/curriculum-guide.git (fetch)
origin	git@github.com:ds-modules/curriculum-guide.git (push)
$ git remote rename origin upstream
$ git remote add origin git@github.com:<your github username>/curriculum-guide.git
$ git remote -v
origin	git@github.com:<your github username>/curriculum-guide.git (fetch)
origin	git@github.com:<your github username>/curriculum-guide.git (push)
upstream	git@github.com:berkeley-dsep-infra/curriculum-guide.git (fetch)
upstream	git@github.com:berkeley-dsep-infra/curriculum-guide.git (push)
```

The raw commands to copy and paste are below:
```
cd curriculum-guide.git
git remote -v
git remote rename origin upstream
git remote add origin git@github.com:<your github username>/curriculum-guide.git
git remote -v
```

Now you can sync your local repo from `upstream`, and push those changes to
your fork (`origin`):
```
git checkout main && \
git fetch --prune --all && \
git rebase upstream/main && \
git push origin main
```

## Procedure
When making changes to anything in this repo, always work in a fork and on a
feature branch.  You should also make sure that your local repo is up-to-date
with this one (upstream) prior to making and committing changes. This is
because other contributors may have pushed changes after you last synced with
this repo.

```
git checkout main && \
git fetch --prune --all && \
git rebase upstream/main && \
git push origin main
```

To create a new feature branch and switch to it, run the following command:
```
git checkout -b <branch name>
```

Make changes to files in the faq or general or technology or workflow directories. The pages and corresponding files can be found in _toc.yml. Add any new pages to _toc.yml.

After you make your changes, you can use the following commands to see
what's been modified and check out the diffs:  `git status` and `git diff`.


When you're ready to push these changes, first you'll need to stage them for a
commit:
```
git add <file1> <file2> <etc>
```

Commit these changes locally:
```
git commit -m "commit description"
```

Now push to your fork:
```
git push origin <branch name>
```

Once you've pushed to your fork, you can go to the
[Curriculum Guide repo](https://github.com/ds-modules/curriculum-guide)
and there should be a big green button on the top that says `Compare and pull request`.
Click on that, check out the commits and file diffs, edit the title and
description if needed and then click `Create pull request`.

Once you create a pull request, a github action will run which will build the jupyterbook
and publish it to https://ds-modules.github.io/curriculum-guide/intro.html as a public facing 
website. Github action will fail if there are issues with the commit.

# Recommended reading
If you are new to `git`, or just want to learn a bit more about it, I highly
recommend taking a look at the official [`git` online book](https://www.git-scm.com/book/en/v2).

Specifically, please read/review the following chapters:
1. [Chapter 1](https://www.git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
2. [Chapter 2](https://www.git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
3. [Chapter 3](https://www.git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell)
4. [Chapter 5](https://www.git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows)
5. [Chapter 6](https://www.git-scm.com/book/en/v2/GitHub-Account-Setup-and-Configuration)


