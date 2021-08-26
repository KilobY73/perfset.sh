# perfset.sh
Automatic toggle performance mode and powersave mode in a shell script file
******
cpupower must be installed first, xbacklight is also needed for visual feedback.

This shell script file can automatically detect the scaling governor that CPU is using now and change it from performance to powersave or powersave to performance.


When switching to performance, the backlight will be turned up a bit (won't if xbacklight isn't installed).
When switching to powersave, the backlight will be turned down a bit (won't if xbacklight isn't installed).

******
Usage:
Execute it directly in a terminal, such as "./perfset.sh" "bash perfset.sh" "source perfset.sh".

Binding a shortcut key such as Fn+Q with the script may make it works like the performance key that Lenovo provided in Windows.
