
<!-- README.md is generated from README.Rmd. Please edit that file -->
msaR
====


msaR is a an [htmlwidgets](https://github.com/ramnathv/htmlwidgets) wrapper of the [BioJS MSA viewer](https://github.com/wilzbach/msa) javascript library. msa will pass alignments to the BioJS MSA 

## updates & new installation instructions
This fork adjusts a few of the default settings in the msaR package.
This version has NOT been committed to CRAN.
You will need to have the following packages installed as well: Rtools, Rcpp, devtools, htmlwidgets

To install this package:
```
devtools::install_github('jkorstia/msaR')
  ## When prompted during installation of msaR, do not install any updates.
```
Running msaR is easy:
```
library(msaR)
msaR("file.fa") 
  ## Note: file.fa must be located in your current working directory
```

To save the output to an html file:
```
library(htmlwidget)
y=msaR("file.fa")
saveWidget(y, "file.html")
```

### License

This project is licensed under the [Boost Software License 1.0](https://github.com/wilzbach/msa/blob/master/LICENSE).

> Permission is hereby granted, free of charge, to any person or organization obtaining a copy of the software and accompanying documentation covered by this license (the "Software") to use, reproduce, display, distribute, execute, and transmit the Software, and to prepare derivative works of the Software, and to permit third-parties to whom the Software is furnished to do so, all subject to the following:

If you use the MSAViewer on your website, it solely requires you to link to us
