# Using Tesseract on Windows

This document outlines steps for converting pdf files into txt files on Windows 10.

## Required Software

Install the following tools. The software below can be used through the Windows commandline.

1. [Imagemagick](https://imagemagick.org/script/download.php#windows), Windows Installer - converts pdf files into images
2. [Tesseract](https://github.com/UB-Mannheim/tesseract/wiki), Windows Installer - converts images into txt files through ocr
3. [Ghostscript](https://www.ghostscript.com/download/gsdnld.html), Windows Installer - a requirement for imagemagick

## Making Commands Available

After installation, specify where these tools have been installed so that they can be executed without having to use the entire location of the file (add the install locations to the `path`):

1. press the windows key to search
2. start typing environment
3. click on "edit environment system variables"
4. click on "Environment Variables"
5. choose "Path"
6. click on "Edit"
7. click on "New"
8. click on "Browse"
9. browse to the installation directory of tesseract (likely under `c:\Program Files`)
10. click on OK through all of the windows
11. do this again for ghostscript (likely under `gs`), starting at step 7
12. do this again for imagemagick (likely under `ImageMagick`)

![set environment variables](path.gif)

