# Download Jupyter Notebook as a PDF

Downloading Jupyter Notebooks (.ipynb files) as PDF can be slightly confusing given the gazillion options presented in the notebook UI. [nbconvert](https://github.com/jupyter/nbconvert) package converts notebook files (ipynb) to varied file formats which includes PDF, PNG etc...The options to download have changed recently due to the recent migration to Notebook 7 and Lab 4.

If you are using https://datahub.berkeley.edu/ then choose the following option
File -> Save and Export Notebook As -> Webpdf

```{figure} ../images/download_webPDF.png
:width: 500px
:align: center
:name: Download Jupyter Notebook as Web PDF
```

If you are using any other hub than https://datahub.berkeley.edu/, then choose the following option,
File -> Save and Export Notebook As -> PDF

```{figure} ../images/download_PDF.png
:width: 500px
:align: center
:name: Download Jupyter Notebook as PDF
```

```{note}
We recommend instructors/students to not use the "File -> Save and Export Notebook as -> Latex" option as it has historically led to "500 internal server error"message for some of our users (like [this](https://github.com/berkeley-dsep-infra/datahub/issues/2664)).
```
