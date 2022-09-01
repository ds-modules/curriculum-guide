# Use Quarto to produce scientific and technical documentation

Quarto is the latest update to the R Studio interface which allows creating scientific and technical documentation which instructors can use as part of their coursework. Quarto generates .qmd files which is used to produce publication worthy documentation. Quarto uses knitr when R is executed inorder to produce .qmd files.

```{figure} ../images/quarto.MOV
:width: 500px
:align: center
:name: Convert R markdown assignments/labs with quarto to produce pdfs
```
Stat 20 instructor Andrew Bray uses Quarto to generate stat20.org which sits on top of netlify which internally uses Quarto as part of the CI/CD. There is also a quarto component in the gradescope autograder as the container infrastructure needs to simulate Datahub environment inorder to run the code containing .qmd files.



