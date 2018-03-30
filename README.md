# mIRC-Scripting-Language-for-Sublime-Text
Updated for mIRC 7.52 (March 2018)

This is my attempt at creating a Sublime Text 3 syntax highlighter for mIRC scripting language.  All $vars and /commands listed in the mIRC help file index should be parsed.  Some undocumented $vars and /commands may be parsed, but I'm sure there's a few that I missed.  Create an issue if any keywords/commands are missing.

- User $variables and mIRC $variables are styled separately.
- User /commands and mIRC /commands are styled separately.
- User .commands and mIRC .commands are styled separately.
- on* and raw events are styled.
- Both ; and /* comments are parsed.

Regex is a little rudimentary, but should work in most cases.  Create a new issue if you encounter any errors and I will try to correct.

To install:

1. Copy mIRC-msl.sublime-syntax to Sublime\Data\Packages\User folder.

You may need to create the Packages\User folder.

![Alt text](screenshots/Install-screenshot.png)


A slightly modified theme has been provided in the Extras folder that supports all features of the highlighter. Themes should support the following scopes to support all styles of this highlighter:
1. comment.line.double-slash
2. constant.numeric
3. constant.numeric.line-number.find-in-files
4.entity.name.class
5. entity.name.function
6. entity.name.tag
7. Keyword.control
8. keyword.operator
9. punctuation.definition.comment
10. string
11. variable.parameter

![Alt text](screenshots/screen1.png)
![Alt text](screenshots/screen2.png)
