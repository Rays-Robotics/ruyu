<!--
SPDX-FileCopyrightText: 2024 suyu Emulator Project
SPDX-License-Identifier: GPL-3.0-or-later
-->
# Migrating from suyu... /!\ DO NOT FOLLOW THIS GUIDE! DOING THIS WILL BREAK THE PROGRAM. /!\

When coming from suyu, the migration is as easy as renaming some directories.

## Windows

Use the run dialog to go to `%APPDATA%` or manually go to `C:\Users\{USERNAME}\AppData\Roaming` (you may have to enable hidden files) and simply rename the `suyu` directories and simply rename those to `ruyu`.

## Unix (macOS/Linux)
Similarly, you can simply rename the folders `~/.local/share/suyu` and `~/.config/suyu` to `ruyu`, either via a file manager or with the following commands:
```sh
 $ mv ~/.local/share/suyu ~/.local/share/suyu
 $ mv ~/.config/suyu ~/.config/suyu
```
There is also `~/.cache/suyu`, which you can safely delete. Suyu will build a fresh cache in its own directory.

### Linux
Depending on your setup, you may want to substitute those base paths for `$XDG_DATA_HOME` and `$XDG_CONFIG_HOME` respectively.

## Android
TBD
