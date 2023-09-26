# Creating Accessible Notebook Experience

Improving the accessibility of the notebook experience has consistently been a key priority for the Datahub infrastructure team. This focus stems from the fact that notebooks have presented significant accessibility challenges, including limited compatibility with screen readers and keyboard navigation, difficulties in interpreting content due to color contrast issues, and non-compliance with the [WCAG 2.0 AA standards](https://www.ucop.edu/electronic-accessibility/standards-and-best-practices/levels-of-conformance-a-aa-aaa.html) mandated by the University.

Enhancing the accessibility of the notebook experience involves addressing multiple dimensions:

- Ensuring the accessibility of the interface, as exemplified by Lab 4 and Notebook 7.
-  Enhancing the accessibility of the content within notebooks.

## Enhancing the accessibility of the notebook interface:

The Datahub team constantly collaborates with Jupyter developers to incorporate accessibility enhancements into both the Notebook and Lab interfaces. In that spirit,we encourage instructors to integrate Lab 4 and Notebook 7 into their teaching workflows, as these releases include the latest accessibility enhancements.

### JupyterLab 4.0: 

A number of accessibility improvements have been made in JupyterLab 4.0, including improved screen reader and keyboard navigation, more ARIA roles and labels, and a hamburger menu that collapses if there is not enough space to display all items. You can read more about the features of Lab 4 in the blogpost titled ["JupyterLab 4.0 is here"](https://blog.jupyter.org/jupyterlab-4-0-is-here-388d05e03442). Lab 4 has undergone extensive testing with Data 100 summer 23 instructors within a new hub, and the overall experience has been positive, with the exception of real-time collaboration, which may require further attention.

### Jupyter Notebook 7.0:

The Jupyter Notebook 7.0, set to become the new default notebook interface, is constructed using reusable components derived from Jupyter Lab 4.0. As part of this transition, both the classic notebook and retro notebook will eventually be replaced. Notably, the accessibility enhancements introduced in Lab 4.0 will also be incorporated into Notebook 7.0. For more details on Notebook 7.0, you can refer to the blog post titled "[Announcing Jupyter Notebook](https://medium.com/jupyter-blog/announcing-jupyter-notebook-7-8d6d66126dcf) 7."

## Enhancing the accessibility of the content within Jupyter notebooks:

There are scenarios where notebooks are designed to be inaccessible. This could include issues with alt text, captioning the images, color contrast issues in the image etc.. One can avoid such accessibility issues by following the best practices recommended to create accessible notebooks.

Sharing couple of resources from the [Iota School](https://github.com/Iota-School) team who has compiled the best practices for creating accessible notebooks into checklists and tips,

- [Checklist](https://iota-school.github.io/notebooks-for-all/exports/resources/event-hackathon/notebook-authoring-checklist/) for notebook authoring
- [Tips](https://iota-school.github.io/notebooks-for-all/exports/resources/event-hackathon/accessibility-tips-for-jupyter-notebooks/#visualization-accessibility) for notebook authoring

#### Export notebook to html format:

The editable notebook format (.ipynb) is inaccessible for screen readers and keyboard navigation. Much effort has been made to Lab 4 and Notbook 7 to overcome some of the barriers to accessibility. However, it is still not 100% accessible at the moment. To improve the readability of the notebooks, It is recommended that .ipynb files are converted to .html files which are largely designed for web interface and has a more accessible experience. PDFs are generally inaccessible in comparison to html format from a readability standpoint.

[Nbconvert](https://github.com/jupyter/nbconvert) is a  tool that converts notebooks to various formats including html which improves readability. The command for converting notebooks from .ipynb to html is

`$ jupyter nbconvert --to html mynotebook.ipynb`

One can also customize the themes, font types, sizes etc. as part of the notebook inorder to improve the accessibility. 

#### Notebook Themes: 

Jupyter Classic Notebook and Lab have 3rd party themes that give more control to the notebook developers to customize the notebook themes and improve accessibility as a result . 

[JupyterLab-Accessible-Themes](https://github.com/Quansight-Labs/jupyterlab-accessible-themes) is a lab theme that allows notebook creators to customize the lab experience. There are two different types of themes which are included as part of this package, 
a) Pitaya Smoothie and 
b) Github Light. Both the themes are WCAG 2.1 AAA compliant and have been recommended by the Jupyter a11y community. However, these themes are not compatible with classic notebook interface.

You can install this theme by running the following command 

`!pip install jupyterlab-accessible-themes==0.1.1`
or 
`conda install -c conda-forge jupyterlab-accessible-themes`

Once installed, you can enable this theme by the following steps,
- Save the notebook and restart the kernel by selecting Kernel -> Restart Kernel
- Select `Github Light theme` by selecting Settings -> Theme -> Github Light and/or `Pitaya Smoothie theme` by selecting Settings -> Theme -> Pitaya Smoothie

[Jupyter Themes](https://github.com/dunovank/jupyter-themes) is a notebook theme that offers 7 different types of themes to customize the classic notebook experience. This theme only works with classic notebook interface and is not compatible with JupyterLab and the Notebook 7.0. 

You can install themes by following command,
`!pip install jupyterthemes`

The different types of themes  are onedork, grade3,  oceans16, chesterish,  monokai, solarizedI,  solarizedd. You can explore these themes using the documentation in [this web page](https://github.com/dunovank/jupyter-themes). If you are looking for JupyterLab equivalent for those themes then you can explore JupyterLab [Legos UI](https://github.com/dunovank/jupyterlab_legos_ui) and [Darkside UI](https://github.com/dunovank/jupyterlab_darkside_ui)

#### Jupyter Font: 

You can use the [JupyterLab fonts](https://github.com/deathbeds/jupyterlab-fonts) package to customize the fonts used in the notebook.

## Enhancing the accessibility of content in the R notebooks:

If you are using R/RStudio as part of your instructional workflow then please check the following resources that provide better ways to make notebook content accessible,

- [Customize themes in R Studio](https://support.posit.co/hc/en-us/articles/115011846747-Using-Themes-in-the-RStudio-IDE)
- [BrailleR: R package that allows blind people understand plots better](https://cran.r-project.org/web/packages/BrailleR/index.html). Here is an [example of BrailleR package](https://cran.r-project.org/web/packages/BrailleR/vignettes/Ex1histograms.html)
- [Sonify: R package converts images into audio representation](https://cran.r-project.org/web/packages/sonify/index.html). Here is an [example for sonifying a data](https://jooyoungseo.com/post/ds4blind/)
- The [TactileR: R package for creating tactile graphics for users with visual impairments](https://github.com/jooyoungseo/tactileR). Here is an [example for tacticleR](https://jooyoungseo.github.io/project/tactiler/)
- [Adding alt text content for images produced by knittR](https://posit.co/blog/knitr-fig-alt/)
- [AccessRMD is the package to improve accessibility of RMD files](https://cran.r-project.org/web/packages/accessrmd/accessrmd.pdf)

Improving accessibility in Jupyter notebooks is an ongoing process that involves attention to both the structural aspects of the content and the interactive elements within the notebooks. It's important to prioritize accessibility to ensure that your content is inclusive and usable by a broad audience.
