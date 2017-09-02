# JupyterHub

## What is JupyterHub?

If you have worked with Jupyter notebooks before, you probably used a local installation. Jupyter notebooks can be created, run, and stored on your personal computer. In order to do all this, you have to install several different programs, such as Python, the Jupyter module, etc. The installation process can be very tedious and error-prone. Even after you have finished installing everything, you may still see errors in the future for various reasons \(versions of software become outdated, you install conflicting software, etc.\). To avoid the frustrations of setting up and maintaining the programming environment needed for Jupyter notebooks, we set up a JupyterHub for use in DSEP courses.

The term JupyterHub refers to the infrastructure set up on datahub.berkeley.edu. This site provides both cloud-based internet storage and computation power for notebooks. Instructors and students can work on and store assignments entirely through JupyterHub. No local installation of Python, Jupyter, etc. is needed. All you need is a browser to get started! This allows students in Data 8 and connector courses to start working on notebooks from day one.

## Why does JupyterHub exist?

Working on JupyterHub provides a number of benefits, especially in an introductory course:

* Students never have to do any setup or installation. JupyterHub removes the burden of setting up and maintaining a development environment.
* All students and instructors use the same computing environment.
* Work stored in the cloud and can be accessed from any computer. 
* All students have access to the same compute power, regardless of the machine they are using. For example, students without personal computers can use library computers without being at a disadvantage in the course. 

## Differences from local installation?

| **JupyterHub** | **Local Setup** |
| :--- | :--- |
| Needs an internet connection | Does not need an internet connection |
| Limited resources \(disk and RAM\) | Unlimited resources \(limited only by your computer\) |
| System-wide installation done by admins | You can install anything you want |
| You can only access files in your account | You can maybe access all files \(if you are an admin\) |
| If things break, we fix them :\) | If things break, you have to fix them :\( |

## Overview of the Internals

The first time you logs in to JupyterHub, a personal account is created for you. You will get your own filesystem so you only have access to the files in your personal account. **Modifications to files in your personal account do not affect anyone else's files. **Unless you are an admin, you cannot access another account's files. This applies to everyone working on JupyterHub, which means a given student cannot access another student's work.

## Getting Access

Anyone with a Berkeley credentials has access to the JupyterHub at `datahub.berkeley.edu`. If you are having difficulties with logging in, please make sure that you are using the correct JupyterHub URL and a berkeley.edu email to login. Please post on Piazza if you are unable to solve JupyterHub access issues.



