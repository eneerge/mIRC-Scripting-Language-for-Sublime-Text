# mIRC-Scripting-Language-for-Sublime-Text
Updated for mIRC 7.52 (April 2018)

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
Autocomplete will work for all /commands and $identifiers.  When completing, the full syntax will be printed so that you can tab through each portion of the command/identifier.

Installation
------------

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

Please see the provided theme to see all implemented features. If you prefer to use another theme, file an issue and I'll see if I can modify the theme to work.  Additionally, you can use the following to modify it yourself or create a new one: https://tmtheme-editor.herokuapp.com/#!/editor/theme/Monokai

![Alt text](screenshots/screen1.png)
![Alt text](screenshots/screen2.png)

Bugs
---------------
Let me know if you find any bugs by submitting an Issue.

IRC Support
--------------
- #Computers @ EFNet
- #mIRC @ EFNet

Special Thanks
--------------
[Peace and Protection Script](https://github.com/solbu/Peace-and-Protection/) - Lots of complex code from this project that I use to test the highlighter.
