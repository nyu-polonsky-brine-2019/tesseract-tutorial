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

See the screencap below.

![set environment variables](path.gif)

## Testing Commands

Test the installation and configuration of the path variables by using cmd.exe and typing in commands. Try doing the following to verify that everything is working correctly:

1. press the windows key to search
2. type in cmd.exe
3. click on "cmd.exe"
4. you should now see a window with a black background and a prompt where you can enter commands
5. type in the following commands
  * `magick`
  * `tessseract`
6. both commands should result in some text showing example usage of each tool
7. if example usage does not apper...
  * ensure that all tools have been installed
  * go back and check the system environment variables -- specifically "Path"

See the animated gif below for expected output.
