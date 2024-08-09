# Use Quarto to produce scientific and technical documentation

Quarto is an open-source publishing system that is particularly valuable for instructors who want to create dynamic, interactive course materials. Whether you're developing lecture notes, assignments, or entire textbooks, Quarto provides a powerful, flexible platform that integrates code, data, and narrative, making it ideal for educational settings. It supports a variety of programming languages, including R, Python, Julia, and Observable JavaScript, enabling instructors to design course content that actively engages students through hands-on coding exercises and real-time data analysis.

```{figure} ../images/Quarto.gif
:width: 500px
:align: center
:name: Convert R markdown assignments/labs with quarto to produce pdfs
```

### Example Usecases

##### 1. Creating Interactive Lecture Notes
Use Case: Developing lecture notes that integrate code, data, and narrative.
How Quarto Helps: Quarto allows you to write notes in Markdown (.qmd files) with embedded code snippets. These snippets can generate live outputs like tables, plots, and calculations directly within the notes.

##### 2. Building Course Websites
Use Case: Hosting all course materials online in a single, accessible location.
How Quarto Helps: Use Quarto to render your Markdown files into a static site, which can be deployed on platforms like Netlify. This site can include lecture notes, assignments, schedules, and more.
Eg: Stat 20 instructor Andrew Bray uses Quarto to generate stat20.org. Quarto is used to create and manage course materials, which are then rendered into a static website. This website is deployed on Netlify, a popular platform for hosting and deploying static sites. Netlify’s Continuous Integration/Continuous Deployment (CI/CD) pipeline automates the process of building and deploying your site whenever you update your Quarto files. This ensures that any changes you make to your course materials are automatically reflected on the live website without additional manual steps.

##### 3. Designing Assignments and Projects
Use Case: Creating assignments where students interact with code and data directly.
How Quarto Helps: Quarto enables you to build assignments in .qmd files that include executable code. Students can run and modify this code to complete their tasks, making the assignments more interactive and practical.

##### 4. Automating Grading with Gradescope
Use Case: Efficiently grading assignments that involve coding and data analysis.
How Quarto Helps: Integrate Quarto into the Gradescope autograder to automatically run and check the code in student submissions. The autograder can simulate environments like Datahub, ensuring consistency in grading.

##### 5. Authoring Books and Manuals
Use Case: Writing textbooks, lab manuals, or comprehensive guides.
How Quarto Helps: Quarto supports long-form content creation, allowing you to compile multiple .qmd files into a cohesive book. You can include live code examples and data analysis, making your book interactive.


### General Workflow for Beginner Instructors

Imagine you’re preparing a lecture on data visualization. You start by writing your notes in a simple Markdown file (.qmd), adding a few basic code examples that generate charts. You then use Quarto to render these notes as a PDF handout and an HTML page for your course website. 

### Quarto Command-Line Conversion

##### Convert Jupyter notebook and Quarto Markdown file to HTML

```{code}
quarto render my-notebook.ipynb --to html
```

The above command converts your Jupyter Notebook (.ipynb) into an HTML file.

```{code}
quarto render my-document.qmd --to html
```
The above command converts your Quarto Markdown file (.qmd) into an HTML file.


##### Convert Jupyter notebook and Quarto Markdown to PDF

**Option 1:**

```{code}
quarto render my-homework.ipynb --to pdf
```
The above command converts your Jupyter Notebook (.ipynb) into a PDF file.

**Option 2:**

```{code}
quarto render my-homework.ipynb --to typst
```

The above command converts your Jupyter Notebook (.ipynb) into a PDF file with a much cleaner output. It uses typst underneath.

```{note}
Typst is a modern typesetting system designed to provide a user-friendly alternative to traditional typesetting tools like LaTeX. It is intended for authors, researchers, and anyone who needs to produce documents with precise formatting and layout control, but without the steep learning curve often associated with traditional typesetting systems. For more details, check out [typst webpage](https://typst.app/)
```

##### Convert qmd file to PDF

```{code}
quarto render my-document.qmd --to pdf
```

The above command converts your Quarto Markdown (. qmd) into a PDF.


For more information about Quarto, Read [here](https://quarto.org/)

```{note}
Quarto can be used in integration with Jupyter Lab. Read more about it [here](https://quarto.org/docs/tools/jupyter-lab.html)
```

### Quarto integration with IDE

Quarto integrates seamlessly with several popular Integrated Development Environments (IDEs) such as RStudio, VSCode and JupyterLab. You can visit this [website](https://quarto.org/docs/get-started/) to learn more about how it integrates with IDEs.

**RSudio:** In RStudio, you can create, edit, and render Quarto documents (.qmd files) directly, leveraging its rich IDE features. 
**Jupyter:** In JupyterLab, you can convert Jupyter notebooks to various formats using Quarto's command-line tools, enhancing interactive notebook workflows.
**VSCode:** Check whether VSCode and [VSCode Quarto extension](https://marketplace.visualstudio.com/items?itemName=quarto.quarto) is enabled in the hub. If yes, you can render and preview quarto documents. You can have syntax highlighting and command line tools to convert to varied documents. 