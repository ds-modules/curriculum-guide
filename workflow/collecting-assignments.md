# Collecting and Grading Assignments

We recommend using [OK](https://www.gitbook.com/book/gunjanbaid/dsep-guide/edit#) for assignment submission and grading. OK is a great tool that allows students to submit notebooks by just running one cell, without having to do any uploads or downloads. More details on OK can be found below.

If you choose not to use OK, you can also have students submit assignments through bCourses. Students can download the assignments from JupyterHub in the original `.ipynb` format, or other formats such as PDF, and then upload them to bCourses.

## OK

[OK](https://okpy.org/) is a tool that contains functionality for submitting and grading notebooks. OK can be used to test code in the notebooks, submit assignments by just running one cell, and grade submissions through the online interface. OK has many advanced features that you can learn more about through their website. This guide will cover just the basics of using the system. There are two parts that you will interact with when using OK for your classes: the OK web interface at `okpy.org` and configuration files that are needed for each assignment. The web interface will be used for initial course setup, adding assignments to OK, and grading. The configuration files are needed to run tests and submit notebooks from JupyterHub.

### Initial Course Setup

To get started with OK, you must first create a course on the OK website. Go to [okpy.org](https://www.gitbook.com/book/gunjanbaid/dsep-guide/edit#), scroll to the bottom of the page, and click on the `REGISTER YOUR COURSE` button to follow the steps for creating a new course. The steps should be fairly straightforward, but as always, feel free to post on [Piazza](https://piazza.com/berkeley/other/cs97) if you run into any trouble.

![](/assets/create-course.png)

### Using OK

After you have finished the initial course setup, below are the steps for setting up an assignment.

1. Create an entry for the assignment on OK site
2. Create a folder for the assignment. This folder will contain the files mentioned in steps 3-5.
3. Create a `.ok` configuration file for the assignment
4. Create a tests folder with at least one test file and an `__init__.py` file
5. Add OK setup code to Jupyter notebook assignment

If you are setting up `lab01`, for example, you should have a folder of content with the following structure:

```
lab01/
    lab01.ipynb
    lab01.ok
    tests/
        __init__.py
        q1.py
```

Note: Even if you are not using tests for your assignment, you will still need to have a tests folder with some placeholder files.

While this process might be a bit tedious the first time, it gets much simpler. You usually do not need to create the configuration files from scratch. You can reuse old files and change a few of the lines. To help you get started, we have set up some [template files](https://github.com/gunjanbaid/course-repo-example/tree/master/fa17/hw/hw02). Some of the steps above are outlined in more detail below.

#### 1. Create an entry for the assignment on OK site

Once you have created your course, you should be able to view it at [okpy.org/admin/course/](https://okpy.org/admin/course/).

#### 3-4. Create configuration file, tests folder

#### 5. Add OK code to notebook



