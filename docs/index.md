--- 
title: "Bookdown Example"
author: "481 Student"
date: "2020-09-18"
site: bookdown::bookdown_site
---

# Preface {-}

This is an example of using bookdown. When you first clone a repo from it as a template, the docs folder only includes this preface (from index.Rmd). That's because I built the book to initially only include this preface (so that's all you'll see in GitHub Pages as well). You'll see that in the main project folder there are two additional RMD files, "01-RegressionOutputTables.Rmd" and "02-LeafletMap.Rmd". When you build the book, the output for these two files will be included as two chapters. This demonstrates that you were able to build the book successfully. 

*A quick note about these two chapters:*

THese two chapters are two RMD files from Econ 380. The first has examples of displaying regression output and graphs. The second has an interactive map. These files demonstrate two ways of reading in data.

 In the first chapter, data is read in from a CSV file ("ceo.csv"). We will always put data into a folder named "data" that we place in the main project folder. This means we always use `data/filename` to read in the data, for example, `read.csv("data/ceo.csv")`. Then we can include "data" in the ".gitignore" file so that Git ignores it. Some of the data files will be really large. This allows us to avoid pushing and pulling the data from GitHub. It makes everything in RStudio much quicker because Git doesn't have to examine large data files to determine if they've changed. And some of the data files might be too large to store in GitHub even if we didn't mind waiting. Following this convention  means you have to manually create the data folder and put the data files in that folder. For the data I give you, I'll post it in Moodle in a Zip folder. 

In the second RMD file (with the map), data is read in directly from a URL. 

We will always use this basic setup. ALways open RStudio by opening the .RProj folder so that the working directory is set correctly. Always put a "data" folder in the main project folder and open data using "data/filename", for example, `read.csv("data/ceo.csv")`. 

