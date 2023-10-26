# Instructional Design Best Practices for Creating Jupyter Notebooks (WIP doc)

Designing an ideal strategy for developing and utilizing Jupyter notebooks as part of your pedagogy can be a challenging exercise. Here are some inputs on the best practices that you can consider while developing your notebook strategy,

- Identify the learning outcomes for your course/module
	- Do you need students to learn a specific programming language?
	- Do you need students to learn a technology specific installation process?
- Choose an ideal  pedagogical strategy to deliver your notebook. Detailed below in the tabular column  are the list of pedagogical approaches you can repurpose for your course. Eg:
	- Have a text to code ratio of 3:1
	- Explain the ouput of the cell in the text annotation above each cell
	- Have an intro Jupyter notebook which focuses on exposing students to syntactical elements of the programming language
- Identify the technology requirements

### Pedagogical strategies for notebook creation
| Pedagogical Approach Name | Course Name |  Notebook Example | Pedagogical Approach Description
| ---- | ----------- | ------ | ------- |
| Cell Execution | Data 101 (Data Engineering) | [Lecture 2 Notebook](https://fa23.data101.org/resources/assets/lectures/lec02/lec02.html) | Students use this notebook to learn  how to connect to a Postgres database hosted in a cloud server. The pedagogical approach followed is to do "Shift-Enter" to execute all the cells and understand how data gets stored in the database |
| Fill in with Code | Data 101 (Data Engineering) | [Project 2 Notebook](Project 2 Notebook) | Students evaluate their understanding by completing the sql query which has been left incomplete as part of the assigment. Through this approach students can test their understanding and identify gaps in their knowledge | 
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
- Github repositories referenced above
- 


