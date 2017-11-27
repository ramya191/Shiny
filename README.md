# Shiny

This is an example application for Shiny. The main purpose of this example is to illustrate how to run Shiny apps from a remote source. There are many ways to download and run it:

library(shiny)

# Easiest way is to use runGitHub
runGitHub("shiny_example", "rstudio")

# Run a tar or zip file directly
runUrl("https://github.com/rstudio/shiny_example/archive/master.tar.gz")
runUrl("https://github.com/rstudio/shiny_example/archive/master.zip")

To run a Shiny app from a subdirectory in the repo or zip file, you can use the subdir argument. This repository happens to contain another copy of the app in inst/shinyapp/.

runGitHub("shiny_example", "rstudio", subdir = "inst/shinyapp/")

runUrl("https://github.com/rstudio/shiny_example/archive/master.tar.gz",
  subdir = "inst/shinyapp/")
