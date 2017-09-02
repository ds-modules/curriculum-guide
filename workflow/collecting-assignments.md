# Collecting and Grading Assignments

We recommend using [OK](https://okpy.org) for assignment submission and grading. OK is a great tool that allows students to submit notebooks by just running one cell, without having to do any uploads or downloads, shown below.



If you choose not to use OK, you can also have students submit assignments through bCourses. Students can download the assignments from JupyterHub in the original `.ipynb` format, or other formats such as PDF, and then upload them to bCourses.

## OK

[OK](https://okpy.org/) is a tool that contains functionality for submitting and grading notebooks. OK can be used to test code in the notebooks, submit assignments by just running one cell, and grade submissions through the online interface. 

OK has many advanced features that you can learn more about through their website. This guide will cover just the basics of using the system. There are two parts that you will interact with when using OK for your classes: the OK web interface at `okpy.org` and configuration files that are needed for each assignment. The web interface will be used for initial course setup, adding assignments to OK, and grading. The configuration files are needed to run tests and submit notebooks from JupyterHub.

### Initial Course Setup

To get started with OK, you must first create a course on the OK website. Go to [okpy.org](https://okpy.org), scroll to the bottom of the page, and click on the `REGISTER YOUR COURSE` button to follow the steps for creating a new course. The steps should be fairly straightforward, but as always, feel free to post on [Piazza](https://piazza.com/berkeley/other/cs97) if you run into any trouble.

![](/assets/create-course.png)

### Using OK

After you have finished the initial course setup, below are the steps for setting up an assignment.

1. Create an entry for the assignment on OK site
2. Create a folder for the assignment. This folder will contain the files mentioned in steps 3-5.
3. Create a `.ok` configuration file for the assignment
4. Create a `tests` folder with at least one test file and an `__init__.py` file
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

#### Step 1: Create an entry for the assignment on OK site

Once you have created your course, you should be able to view it at [okpy.org/admin/course/](https://okpy.org/admin/course/). Go to this page and click on your course.

![](/assets/ok-courses.png)

Click on the `Create Assignment` button on the left side of the page and follow the steps listed.

![](/assets/create-assignment.png)

#### Steps 3-4: Create configuration file, tests folder

For `lab01`, you need to set up `lab01.ok`  and a `tests` folder with an `__init__.py` file and `q1.py`. Below, I have pasted the contents of the [template files](https://github.com/gunjanbaid/course-repo-example/tree/master/fa17/hw/hw02), mentioned above, with added comments on which lines to modify for use with your own course.

##### `lab01.ok`

```
{
  "name": "Homework 2",                    # change this line
  "endpoint": "cal/ds101/su17/hw02",       # change this line with OK info for your course
  "src": [
    "hw02.ipynb"                           # change this line, this is the file to be submitted
  ],
  "tests": {
      "tests/q*.py": "ok_test"
  },
  "protocols": [
      "file_contents",
      "grading",
      "backup"
  ]
}
```

##### `tests` folder

Should contain at least `__init__.py` file and `q1.py` even if you are not using tests. These files are needed to ensure that OK does not error. You can add additional question files, such as `q2.py` and so on.

##### `__init__.py`

This should be blank.

##### `q1.py`

The test in this file is checking whether the value of `x` is equal to 91. `x` is a variable defined somewhere in the notebook corresponding to this test file. You can change the two lines indicated to create a different test.

```
test = {
  'name': '',
  'points': 1,
  'suites': [
    {
      'cases': [
        {
          'code': r"""
          >>> x                          # change this line
          91                             # change this line
          """,
          'hidden': False,
          'locked': False
        }
      ],
      'scored': True,
      'setup': '',
      'teardown': '',
      'type': 'doctest'
    }
  ]
}
```

#### Step 5: Add OK code to notebook

Below is the code needed to import OK, run the `q1.py` test shown above, and submit the assignment. You can change the marked lines to use this code for your own assignments. The original code is found in the `hw02.ipynb` file in the [template files](https://github.com/gunjanbaid/course-repo-example/tree/master/fa17/hw/hw02).

```
# These lines load the autograder tests. 
from client.api.notebook import Notebook
ok = Notebook('hw02.ok')                     # change this line to correct .ok file
_ = ok.auth(inline=True)
```

```
# Test q1
x = 91                                       # change this line to desired test
_ = ok.grade("q1")                           # change this line to desired test file
```

```
# Submit the assignment.
_ = ok.submit()
```



