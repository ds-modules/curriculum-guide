# Download Jupyter Notebook as a PDF

Downloading Jupyter Notebooks (.ipynb files) as PDF can be slightly confusing given the number of options presented in the notebook UI. [nbconvert](https://github.com/jupyter/nbconvert) is the third-party package used to convert notebook files (ipynb) to file formats such PDF,HTML, PNG etc...The options to download notebook as PDF/HTML has changed recently due to the migration from notebook 6 to 7 and Lab 3 to 4.

Choose the following option to download the ipynb file(s) as pdf then choose the following option,

File -> Save and Export Notebook As -> Webpdf

```{figure} ../images/download_notebook_webpdf.png
:width: 500px
:align: center
:name: Download Jupyter Notebook as Web PDF
```

If you choose to download the ipynb file(s) as HTML then choose the following option,

File -> Save and Export Notebook As -> HTML

```{figure} ../images/download_notebook_html.png
:width: 500px
:align: center
:name: Download Jupyter Notebook as HTML
```

```{note}
When it comes to embedding images in Jupyter notebooks so that it is available as part of PDF, there are various methods to include images. Below are the five options to embed an image of an early Mathematica interface.

#### HTML Image Tag

```{code}
<img src="mathematica.png" alt="Early Mathematica Interface" style="width: 250px;" class="center"/>
```

This method uses standard HTML to embed an image. It is straightforward and allows for extensive customization through HTML attributes like style and class.

#### Markdown Image Syntax

```{code}
![mathematica](mathematica.png)
```

Markdown provides a simple syntax for embedding images. This method is concise and ideal for use in Markdown cells in Jupyter notebooks.

#### HTML in Markdown Cell

```{code}
<img src="https://rtl.berkeley.edu/profiles/openberkeley/themes/openberkeley_theme_brand/assets/images/berkeley_wordmark_blue_175x70.svg" alt="Berkeley Logo" style="width: 250px;" class="center"/>
``` 

Embedding an image using HTML within a Markdown cell offers the flexibility of HTML while allowing the cell to remain in Markdown mode. This is useful for more complex styling and alignment requirements.

#### IPython Display Module

```{code}
from IPython.display import display, Image
display(Image(filename="mathematica.png", width=250))\
``` 

The IPython.display module provides functions to display images directly in Jupyter notebooks. 

#### Markdown Image with Attachment

```{code}
![mathematica.png](attachment:5265a161-c705-42fc-a3ed-ec1fde427030.png)
``` 

This method is used to embed an image as an attachment within a Jupyter notebook. It references the image by its attachment identifier, which is useful for images embedded directly within the notebook file.

```
