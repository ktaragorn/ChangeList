Change List (Last Edit) for Sublime Text 2
====================
Navigating between edited locations!
<img src="https://github.com/randy3k/Change-List/raw/master/changelist.png">

Introduction
------------
This plugin aims at recovering the full functionality of Change-List of VI.
* Type ``Change List`` in Command Palette to show Change List panel.
* ``super+;`` or ``g;`` (vinage command mode): go the previous edited location
* ``super+,`` or ``g,`` (vinage command mode): go the next edited location
* Type ``Clear Change List`` in Command Palette to clear Change List.

There are already a few other "LastEdit" plugins . For examples:
* https://github.com/SamPeng87/sublime-last-edit
* https://github.com/khrizt/GotoLastEdit
* https://github.com/abrookins/GotoLastEdit
* https://github.com/Stuk/sublime-edit-history
* https://github.com/optilude/SublimeTextMisc/blob/master/navigationHistory.py
* https://gist.github.com/1993147 

However, they do not keep editing history after the file is saved and closed (as far as I can tell).<BR>
This plugin allows you to navigate between edited locations even the computer is restarted.<BR>
The history is saved to ``Packages/User/Change-List.sublime-settings``.<BR>
For the moment, the last 50 editing history for each file will be saved.<BR>

Note: It is not the Jump List. It means that the cursor always stays in the same file.

Keymap
----------------------
Note that it overwrites the default keymap ``super+,`` for consistency.

TODO
-----------------------
* Don't update change list while undoing.
* Multi cursor support is now limited, only the locataion of first cursor will be saved.
  However, multi cursor editing preserves the history.
