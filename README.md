# perfset.sh
Automatic toggle performance mode and powersave mode in a shell script file
******
cpupower must be installed first, xbacklight is also needed for visual feedback.

This shell script file can automatically detect the scaling governor that CPU is using now and change it from performance to powersave or powersave to performance.


When switching to performance, the backlight will be turned up a bit (won't if xbacklight isn't installed).
When switching to powersave, the backlight will be turned down a bit (won't if xbacklight isn't installed).

******
Usage:
After getting the file, make it executable first by "chmod 755 ./perfset.sh".
Then you may need to change your sudoers file and add "%user ALL=(root)NOPASSWD:/usr/bin/cpupower" at the end of the file in order to make the governor can be changed without password.
Finally you can execute it directly in a terminal, such as "./perfset.sh" "bash perfset.sh" "source perfset.sh".

Binding a shortcut key such as Fn+Q with the script may make it works like the performance key that Lenovo provided in Windows.
