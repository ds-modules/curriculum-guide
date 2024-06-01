# Download Jupyter Notebook as a PDF

Downloading Jupyter Notebooks (.ipynb files) as PDF can be slightly confusing given the numebr of options presented in the notebook UI. [nbconvert](https://github.com/jupyter/nbconvert) is the third-party package used to convert notebook files (ipynb) to file formats such PDF,HTML, PNG etc...The options to download notebook as PDF/HTML has changed recently due to the migration from notebook 6 to 7 and Lab 3 to 4.

If you are using https://datahub.berkeley.edu/ and/or https://r.datahub.berkeley.edu/, then choose the following option to download the ipynb as pdf,

File -> Save and Export Notebook As -> Webpdf

```{figure} ../images/download_webPDF.png
:width: 500px
:align: center
:name: Download Jupyter Notebook as Web PDF
```

```{note}
When using webpdf option, ensure that your images are formatted appropriately so that it gets rendered in the PDF given the issue with [nbconvert](https://github.com/jupyter/nbconvert/issues/1326#issuecomment-1019204102).

Absolute URLs: Images with absolute URLs in the image tag source are rendered in the PDF. Example: <img src="https://data-88e.github.io/assets/images/blue_text.png">.

Relative URLs: Images with relative URLs in the image tag source won't be rendered in the PDF. Example: <img src="blue_text.png">.

Markdown Format: Images added in Markdown format, like 

```{code}
![Macss Logo](blue_text.png)
```
,are rendered in the PDF.

```

If you are using any other hub than the ones mentioned above, choose the following option,
File -> Save and Export Notebook As -> PDF

```{figure} ../images/download_PDF.png
:width: 500px
:align: center
:name: Download Jupyter Notebook as PDF
```

If you choose to download the notebook files as HTML then choose the following option,
File -> Save and Export Notebook As -> HTML

```{figure} ../images/download_HTML.png
:width: 500px
:align: center
:name: Download Jupyter Notebook as HTML
```

```{note}
We recommend instructors/students to not use the "File -> Save and Export Notebook as -> Latex" option as it has historically led to "500 internal server error"message for some of our users (like [this](https://github.com/berkeley-dsep-infra/datahub/issues/2664)).
```
