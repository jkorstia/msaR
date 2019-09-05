
<!-- README.md is generated from README.Rmd. Please edit that file -->
msaR
====

[![Travis Build Status](https://travis-ci.org/zachcp/msaR.svg?branch=master)](https://travis-ci.org/zachcp/msaR) [![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/msaR)](https://cran.r-project.org/package=msaR)

msaR is a an [htmlwidgets](https://github.com/ramnathv/htmlwidgets) wrapper of the [BioJS MSA viewer](https://github.com/wilzbach/msa) javascript library. msa will pass alignments to the BioJS MSA and has a convenience function that will handle the following formats:

1.  A character string which is interpreted to be a fasta file (opened by `ape::read.dna`)
2.  A DNAbin class object (ape)
3.  An XStringSet (Biostrings) including "DNAStringSet", "RNAStringSet", "AAStringSet", and "BStringSet"
4.  An XMultiple Alignment (Biostings) including "DNAMultipleAlignment","RNAMultipleAlignment", and"AAMultipleAlignment"

Any of these types of objects can be passed to msaR to create an html widget. See [the online docs](https://zachcp.github.io/msaR/) for an interactive version of this widget.

## updates & new installation instructions
This fork adjusts a few of the default settings in the msaR package.
This version has NOT been committed to CRAN.
To install this version:
```
git clone https://github.com/jkorstia/msaR.git
R CMD INSTALL msaR
```
Or via [devtools](https://github.com/hadley/devtools)
```
devtools::install_github('jkorstia/msaR')
```

Running msaR is easy:
library(msaR)
msaR("file.fa")

### License

This project is licensed under the [Boost Software License 1.0](https://github.com/wilzbach/msa/blob/master/LICENSE).

> Permission is hereby granted, free of charge, to any person or organization obtaining a copy of the software and accompanying documentation covered by this license (the "Software") to use, reproduce, display, distribute, execute, and transmit the Software, and to prepare derivative works of the Software, and to permit third-parties to whom the Software is furnished to do so, all subject to the following:

If you use the MSAViewer on your website, it solely requires you to link to us
