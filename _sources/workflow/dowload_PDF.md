# Download Jupyter Notebook as a PDF

Do you want to download Jupyter Notebooks (.ipynb files) as a PDF but are confused by the gazillion options available in the notebook UI? We use a package called nbconvert which converts notebook files into different file formats including PDF.The download options have changed recently due to the recent migration to Notebook 7 and Lab 4.

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
We recommend not using the option "Download as Latex" as that has historically led to 500 server errors for a few instructors (like [this](https://github.com/berkeley-dsep-infra/datahub/issues/2664)).
```
