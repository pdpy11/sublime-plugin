# sublime-plugin

This repository contains various utilities for integration of PDPy11 with Sublime Text. I might convert it to a full-blown plugin someday.

These utilities are:

- The build script which allows you to use Ctrl-B to build the program.
- The [syntax highlighting](https://en.wikipedia.org/wiki/Syntax_highlighting) specification, which teaches Sublime Text how to parse assembly.
- The color scheme based on Monokai, which you may or may not find useful. This is a relict more than a necessity.


## Installation

To install the utilities, open the user packages directory of Sublime Text by clicking through `Preferences` -> `Browser Packages...` -> `User` subdirectory. Then extract the files (except README, of course) [from here](https://github.com/pdpy11/sublime-plugin/archive/refs/heads/master.zip) and put them to User.

To switch to the custom color scheme, open the command panel via Ctrl-Shift-P, choose 'Select Color Scheme' and then 'PDPy11'. You can use the same method to switch to the previous color scheme too, if you don't like PDPy11.

The other two features should be enabled automatically.


## Handling problems

If you installed the pdpy11 compiler correctly, the build script should work as is. If it doesn't, open the Sublime console via Ctrl-\` and check if any errors appear when you try to build a program.

If it says anything along the lines of 'pdpy11: No such file or directory', this means you didn't set up PATH correctly. The pdpy11 README describes how this should be done. A robust way to check if everything is installed correctly is to try to run `pdpy11 -h` in the command prompt and see if it shows a help message or an error.
