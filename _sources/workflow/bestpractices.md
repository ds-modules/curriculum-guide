# Instructional Design Best Practices for Creating Jupyter Notebooks (WIP doc)

Designing an ideal strategy to develop and utilize Jupyter notebooks as part of your pedagogy can be a challenging exercise. Here are some inputs on the best practices that you can consider while developing your notebooks,

- Identify the appropriate learning outcomes you want to achieve using Jupyter notebook for your course/module. Some of the questions to consider are,
	- Are the students expected to learn a specific programming language?
	- Are the students expected to learn a new technology/installation process?
	- Will students work together in groups or work independently to solve an assignment
	- Will students work on assignments synchronously during the class or asynchronously after the class?
	-  Will students publish their notebook as a PDF/HTML website/Dashboard/Jupyter Book etc..
	- What kind of datasets are required to achieve the learning outcomes envisioned? 
- Choose an ideal  pedagogical strategy to deliver your notebook. Detailed below in the tabular column  are the list of pedagogical approaches you can repurpose for your course. Eg:
- Identify the technology requirements based on your answers,

### Pedagogical strategies for notebook creation
| Pedagogical Approach Name | Course Name |  Notebook Example | Pedagogical Approach Description
| ---- | ----------- | ------ | ------- |
| Cell Execution | Data 101 (Data Engineering) | [Lecture 2 Notebook](https://fa23.data101.org/resources/assets/lectures/lec02/lec02.html) | Students use this notebook to learn  how to connect to a Postgres database hosted in a cloud server. The pedagogical approach followed is to do "Shift-Enter" to execute all the cells and in the process understand to work with Postgres database. Students read data from the database, run complex queries against the data to perform analysis |
| Fill in with Code | Data 101 (Data Engineering) | [Project 2 Notebook](https://data101.datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Fcal-data-eng%2Ffa23-materials&urlpath=lab%2Ftree%2Ffa23-materials%2Fproj%2Fproj2%2Fproj2.ipynb&branch=main) | Students evaluate their understanding by completing the sql query which has been left incomplete as part of the assigment. Through this approach students can test their understanding and identify gaps in their knowledge | 
| Translate Mathematics to Code | PMB/MCB/BioE C 146 (Data Science for Biology) | [Lecture 8 Notebook](https://github.com/ds-modules/ds4bio/blob/main/lab8/lab08-c146-v01-student.ipynb) | Students learn about dynamic programming in this notebook. They generate fibonacci series and find longest common subsequence using recursive function/dynamic programming and calculate the associated complexity. Here, the students will be codifying mathematical expression to understand the knowledge better |
| Explore APIs | EPS 88 (PyEarth) | [Week 2 Assignment](https://github.com/ds-modules/EPS88-24031-FA23/blob/main/week02_datahubfiles/W02_assignment_Earthquakes.ipynb) | In this notebook, students query a remote server hosted by US Geological Survey Org to get data about areas in the globe where an earth quake has happened and whose magnitude is greater than 5.0. They create a map highlighting  those places |
Hello World | Econ 130 (Economics for Public Policy) | [Intro Jupyter notebook](https://github.com/ds-modules/ECON-130-FA23/blob/main/IntroToR/Intro%20to%20R.ipynb) | Many courses have this intro notebook where student perform basic operations in Python/R to understand the syntax of the programming language. Instructors spend a week helping students get accustomed to the chosen programming language | 
 
### Best Practices/Tips for Notebook Creation

- Have a text to code ratio of 3:1
- Explain the ouput of the cell in the text annotation above each cell
- Have an intro Jupyter notebook which focuses on exposing students to syntactical elements of the programming language

### Credits/References
- [Teaching and Learning with Jupyter](https://jupyter4edu.github.io/jupyter-edu-book/index.html)
- [Best practices for writing and sharing computational analysis in Jupyter notebooks](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6657818/)
- Github repositories of varied repositories referenced above


