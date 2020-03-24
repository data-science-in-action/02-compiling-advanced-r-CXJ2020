---
title: "Problems and Solutions"
author: "CXJ2020"
date: "2020/3/20"
output: pdf_document
---
During the building process, those are some errors I've met and how I solved them.

## Error in cat(paste0(contributors$desc, collapse = ", "))

Solution:Adding `encoding="UTF-8"`to line 224.
The full command is: `contributors <- read.csv("contributors.csv", stringsAsFactors = FALSE,encoding = "UTF-8")`

## Error in loadNamespace(name) : 'emo'

Solution:download *Rtools* to my computer, preferably in disk C, and select "Add Rtools to system PATH". Install the package *devtools*, and then input the command: `library(usethis)`, `library(devtools)`, `devtools::install_github(" Hadley /emo")`

## Error in library(dplyr) or Error in loadNamespace(name) :'sessioninfo'

Solution:Errors like these indicate missing packages. Using `install.packages()` to solve it. The packages I installed are dplyr,sessioninfo,lobstr, devtools, sloop,profvis,bench,ggbeeswarm.

## In system(cmd) : 'make' not found

Solution:Add *Rtools* to the system path, and restart the computer and Rstudio.

## 'xelatex'not Found
Solution:Use tinytex to install TinyTex might can't solve the problem, so I used MiKTeX instead.

## Package fontspec Error: The font 'Inconsolata' and 'Andale Mono' cannot be found.
Solution:Download the Inconsolata font and Andale Mono font, and place them in the C:/Windows/Fonts folder

Through this experience,I have learnt a lot.Thanks for my teacher and classmates.
