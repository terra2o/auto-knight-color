# KDE Plasma automatic night theme switcher
auto-knight-color is a shell script that automatically switches between light and dark colors in KDE Plasma. It uses the color temperature settings from KDE's Night Color feature to determine when to switch themes.

It is intended to be light weight.

## Dependencies
* qdbus6: A tool for sending and reading DBus messages and values. This is used to get the current daylight status from KDE's Night Color feature.
* dbus-monitor: A tool for monitoring DBus messages. This is used to detect changes in the daylight status.
* grep: A tool for filtering text. This is used to filter the output of dbus-monitor for messages about the target color temperature.

## Installation
To use auto-knight-color, you need to have the above dependencies installed. You can then download the script, make it executable and add it as a login script via KDE autostart.

After opening a terminal in the same directory as the script, make it executable with this command:
```
chmod +x auto-knight-color
```


## Customization
You can customize the light and dark colors used by the script by modifying the light_scheme and dark_scheme variables at the top of the script.

## Credit
This project is based on auto-knight by Dmitriy Safiullin (DimseBoms). Changes have been made to modify only the KDE color scheme.
