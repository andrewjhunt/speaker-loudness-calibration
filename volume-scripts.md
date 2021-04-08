# AppleScript for System Volume

Scripts for getting and setting the system volume in MacOS.

Open "Script Editor" which you can find in the Applications ➜ Utilities folder.  Create a new document.

Enter and run a script:

1. Type a script into the upper panel. e.g "get volume settings"
1. Click the Run/Play button
1. Get the result in the lower panel

**Get the current System Volume settings**

Script: `get volume settings`

Result: `output volume:58, input volume:100, alert volume:100, output muted:false`

**Set the current System Output Volume**

Script: `set volume output volume 68`

Result: empty but the volume will change

**Creating convenient volume scripts**

I found it very convenient to create a menu in my system menu bar with all my calibrated volumes.

![](images/volume-scripts.png)

First, enable Apple Scripts in the desktop's menu bar.

1. Open Utilities ➞ "Script Editor"
1. In the app preferences, enable "Show Script menu in menu bar"

Now we create a script for each SPL. The default location for user scripts is `Library/Scripts` in your home directory. Conveniently, the Script Editor menu bar has an option to "Open Scripts Folder" for "User Scripts".

Now...

1. Write your volume script. My calibrated `60dB` system volume is `71` so `set volume output volume 71`
1. File ➜ Save and create `Volume 60dB.scpt`
1. Place the saved script into directory `<home>/Library/Scripts`
1. This volume script should now appear conveniently in your menu bar

Repeat for other volumes.
