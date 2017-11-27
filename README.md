# Shiny

This is an example application for Shiny. The main purpose of this example is to illustrate how to run Shiny apps from a remote source. There are many ways to download and run it:

library(shiny)

# Easiest way is to use runGitHub
runGitHub("shiny", "rstudio")

Or you can clone the git repository, then use runApp():

# First clone the repository with git. If you have cloned it into
# ~/shiny, first go to that directory, then use runApp().
setwd("~/shiny")
runApp()

