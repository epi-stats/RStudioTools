# RStudioTools
R/RStudio Package to use addins in RStudio for data manipulation and simple statistics
RStudioTools will help you get started with the open-source statistical environment R. 
After installation, several new applications (gadgets) are available which can be accessed via RStudio's 'Addins' menu 
(if the toolbar is not visible: 'View' > 'Show toolbar').
Many important tasks can be executed through interactive menus, which will generate automatically the associated R code. 
A minimum screen resolution of 1080 (height) is recommended. 

Requires R v4.0.0 or higher and RStudio v0.99.878 or higher (recommended R v4.1 and RStudio v2023.x)
## Installation
Run the code below in RStudio to install the package 

install.packages(c("miniUI", "rstudioapi"))

install.packages("https://github.com/epi-stats/RStudioTools/raw/master/RStudioTools_0.6.0.tar.gz", repos=NULL, type="source", method="libcurl")

# To open the documentation
```
help(package = "RStudioTools")

vignette("RstudioTools_introduction", package = "RStudioTools")
```
If text or fields in the gadgets are not properly displayed, try one of the following: 
i) adjust height and weight of the viewer pane, 
ii) maximize the RStudio window, 
iii) set Zoom to 100% ( under Tools/Global options/Appearance), 
iv) click the "Show in new window" button to open the gadget in the internet browser.

Note: Some of the tools might not work as expected if the data are imported
from Stata, SPSS or SAS using the haven package.
The following line should resolve the problem:
class(mydata) <- "data.frame" 
If the problem persists, it is always be possible to write the data in ASCII
format and to reload it again:
write.table(mydata, 'mydata.txt')
mydata <- read.table('mydata.txt')
