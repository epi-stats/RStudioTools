# RStudioTools
# R/RStudio Package to use addins in RStudio for data manipulation and simple statistics
# RStudioTools will help you get started with the open-source statistical environment R. 
# After installation, several new applications (gadgets) are available which can be accessed via RStudio's 'Addins' menu 
# (if the toolbar is not visible: 'View' > 'Show toolbar').
# Many important tasks can be executed through interactive menus, which will generate automatically the associated R code. 
# A minimum screen resolution of 1080 (height) is recommended. 

# Requires R v3.3.0 or higher and RStudio v0.99.878 or higher
# Run the script below in RStudio to install the package 

install.packages(c("miniUI", "rstudioapi", "readxl"))

download.file("https://github.com/epi-stats/RStudioTools/raw/master/RStudioTools_0.5.6.tar.gz", "RStudioTools")

install.packages("RStudioTools", repos = NULL, type = "source")

# To open the documentation

help(package = "RStudioTools")

vignette("RstudioTools_introduction", package = "RStudioTools")

# If text or fields in the gadgets are not properly displayed, try one of the following: 
# i) adjust height and weight of the viewer pane, 
# ii) maximize the RStudio window, 
# iii) set Zoom to 100% ( under Tools/Global options/Appearance), 
# iv) click the "Show in new window" button to open the gadget in the internet browser.

