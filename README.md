# mIRC-Scripting-Language-for-Sublime-Text
Updated for mIRC 7.72 (Feb 2023)

This project implements syntax highlighting and autocompletion for mIRC msl.  It currently supports:
- All /Commands
- All $Identifiers
- All on EVENTs
- Goto Loop highlighting
- Popups
- #Groups
- Comments (; and /*)
- @Windows
- Numerics
- User Variables
- Params ($1, $2, etc)
- Operators (ison, iswm, $+, >=, <=, etc)
- Logic (if, else, while, etc)

This project aims to make Sublime Text the premier choice for developing mIRC msl.  If you encounter any problems, please create an issue.

Highlighting
---------------
Highlighting currently supports all commands and identifiers in mIRC.  In addition "on/ctcp/raw events" will also highlight.  I try to cover all cases including: commands on new line, commands inline, commands after a |, commands after a {, etc.  I welcome any suggestions for improvement.

Auto Completion
---------------
Autocomplete will work for all /commands and $identifiers.  They will display in the autocomplete popup.  Additionally,  I have added support for tabbing through the full syntax of /commands through /color (alphabetical).  I am adding support for more and hope to support displaying the full syntax of all remaining commands and identifiers in the future.

Installation
------------
# Option 1 (Package Control)
This package is now available in Package Control.  If you have Package Control installed:
1. Ctrl+Shift+P
2. Install Package
3. mIRC Scripting Language (Highlight and Autocomplete)

# Option 2 (Manual)
1. Copy mIRC-msl.sublime-syntax to Sublime\Data\Packages\User folder.
2. Copy mIRC-msl.sublime-completions to Sublime\Data\Packages\User folder.

You may need to create the Packages\User folder.

![Alt text](screenshots/Install-screenshot.png)


Theme Support
--------
A slightly modified theme has been provided in the Extras folder that supports all features of the highlighter. Themes should support the following scopes to support all styles of this highlighter:
1. comment.line.double-slash
2. constant.numeric
3. constant.numeric.line-number.find-in-files
4. entity.name.class
5. entity.name.function
6. entity.name.tag
7. Keyword.control
8. keyword.operator
9. punctuation.definition.comment
10. string
11. variable.parameter

Please see the provided theme to see all implemented features. If your theme doesn't work, let me know by filing an issue.

![Alt text](screenshots/screen1.png)

Bugs
---------------
Let me know if you find any bugs by submitting an Issue.

IRC Support
--------------
- Eneerge on EFnet

Special Thanks
--------------
[Peace and Protection Script](https://github.com/solbu/Peace-and-Protection/) - Lots of complex code from this project that I use to test the highlighter.
