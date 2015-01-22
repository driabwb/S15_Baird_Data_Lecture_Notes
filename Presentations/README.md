# Presentations README

## About
This directory presently contains all the presentations I have created for Data Engineering and how I turned the Markdown into a PDF slideshow.

## Creating Slideshow
The slide show is created by writing up a Markdown document and running it through pandoc, which converts it.
This can be done easily with some default settings which are in the generate script.

Usage:
> `./generate <Markdown_File_Name>`

Requirements:
* pandoc must be installed
* Latex needs to be installed 
  * (I suspect that only a subset of Latex is needed, but I not sure what is or is not neccessary).