# Sunshine-Set-Resolution
A simple script built around this script (https://superuser.com/a/1661660) to change the screen resolution. Can be used as a global command within Sunshine to set the resolution of the target device based on the client device's width/height (or a custom width/height) with greater reliability than other solutions (from personal experience).

## How to Use
- Download the file
- Within Sunshine's Config -> General settings, scroll to Command Preparations
- Enter the following command for config.do_cmd: powershell.exe -executionpolicy bypass -windowstyle Hidden -file "[SCRIPT LOCATION]" -InputWidth 0 -InputHeight 0
- Enter the following command for config.undo_cmd: powershell.exe -executionpolicy bypass -windowstyle Hidden -file "[SCRIPT LOCATION]" -InputWidth [DEVICE_NATIVE_WIDTH] -InputHeight [DEVICE_NATIVE_HEIGHT]
- Save and Apply the settings
- Start a game

Note that this script can also be used to change the screen resolution on an app by app basis by changing the -InputWidth and -InputHeight parameters to whatever you would like to within each application (under the Application -> [Your desired application] -> Edit -> Command Preparations
