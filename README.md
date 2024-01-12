---
title: "Using SQL and Docker to access NHANES"
date: "2024-01-11"

bibliography: references.bib
output:
  word_document: 
    keep_md: true
  bookdown::pdf_book:
    citation_package: biblatex
  html_document:
    df_print: paged
  pdf_document: null
header-includes: \usepackage{multicol}
link-citations: yes
csl: vancouver.csl
---


## Abstract:

The National Health and Nutrition Examination Survey (NHANES) @Pruim2015 is a widely used and largely publicly available data set.  In our previous work, we described online access to NHANES via the `nhanesA` package (cite).  In this paper we describe our efforts to create a Docker(cite docker)  container that holds the NHANES data in a SQL database together with the R programming language @R-base , a companion R package `phonto` @phonto2023  and additional software tools to support a variety of analyses.  The container can run on very modest hardware (e.g.most laptop computers).   We believe that this resource will be valuable for education and scientific investigation and that it will help build a community of researchers that can more rapidly extend and apply epidemiological methods, thereby increasing the pace of scientific discovery while at the same time greatly improving reproducibility.

Database URL: <https://github.com/ccb-hms/NHANES>

## References

## Appendix

### Summary of functions 
Table 1: List of of the functions of phonto

|Functions            |Descriptions                                           |
|:--------------------|:------------------------------------------------------|
|checkDataConsistency |Check Variable Consistency                             |
|dataDescription      |dataDescription                                        |
|jointQuery           |Joint Query                                            |
|metaData             |Show meta data information                             |
|nhanesQuery          |Query NHANES data from Database                        |
|nonPhenotypes        |non phenotypes data                                    |
|phesant              |simple version of PHEnome Scan ANalysis Tool (PHESANT) |
|unionQuery           |Union Query                                            |
|nhanesHead           |Return the First of an NHANES table                    |
|nhanesTail           |Return the Last of an NHANES table                     |
|nhanesNcol           |The Number of Columns of an NHANES table               |
|nhanesColnames       |Column Names for NHANES tables                         |
|nhanesDim            |Dimensions of NHANES table                             |
|nhanesNrow           |The Number of Rows of an NHANES table                  |

