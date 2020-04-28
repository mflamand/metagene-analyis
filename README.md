This is R Markdown code is a simple tutorial on performing m6A metegane analysis based on previous work from https://github.com/olarerin/metaPlotR.

sample data from Linder et al 2015 (https://www.ncbi.nlm.nih.gov/pubmed/26121403) miCLIP dataset

You can clone/download the whole project and then open the markdown file.

You can download R from Duke's archive download site here : http://archive.linux.duke.edu/cran/ by selection the version for your platform.

R was just updated to version 4.0.0, you download this version, or an older one it doesn't matter.
If you have an older version (3.6.x) it is fine and you don't need to update if you don't want. 

working on a newer version will mean that you are likely to have to compile from source quite a few libraries as they have not already been compiled by CRAN. This is done automatically as long as you have the compilers installed on your machine.

For Windows: on the download page, you will have to select and install base for the R software as well Rtools to compile libraries.

Once installed, within R, you should type `writeLines('PATH="${RTOOLS40_HOME}\\usr\\bin;${PATH}"', con = "~/.Renviron")` to add the path of the compiler to R. 

For MacOS-X you will need to install quite a few things as well:
  1. on new versions, it is possible that you will need to be install XQuartz to use some packagages (https://www.xquartz.org/). It used to be provided by defaults before 10.8
  2. Apple's Xcode developer tools. which again used to be provided. You now have to signup as a developer with Apple
  3. a GNU fortran compiler
you can find details on this page : https://mac.r-project.org/tools/ 
  4. extra libraries indicated on the previous pages. This only be necessary for certain libraries
  
  Normaly, if you try to install a package and it fails, you can inspect the error message to see where it failed and figure out what was missing.


You can then install RStudio, a GUI for R here : https://rstudio.com/products/rstudio/download/#download

When you launch RStudio, it will automatically load the most recent R version detected on the system
