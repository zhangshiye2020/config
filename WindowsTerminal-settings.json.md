# WindowsTerminal Config

**配置路径**
```path
C:%HOMEPATH%\AppData\Local\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe
```
**配置文件**
```json
{
  "$schema": "https://aka.ms/terminal-profiles-schema",

  "defaultProfile": "{0caa0dad-35be-5f56-a8ff-afceeeaa6101}",

  "copyOnSelect": false,

  "copyFormatting": false,

  "profiles": {
    "defaults": {
      "cursorShape": "filledBox",
      "backgroundImage": "ms-appdata:///local/miku.png",
      "backgroundImageAlignment": "bottomRight",
      "backgroundImageStretchMode": "uniform",
      "acrylicOpacity": 0.85,
      "backgroundImageOpacity": 0.6,
      "background" : "#282C34",
      "snapOnInput" : true,
      "useAcrylic" : true,
      "black" : "#282C34",
      "blue" : "#61AFEF",
      "brightBlack" : "#5A6374",
      "brightBlue" : "#61AFEF",
      "brightCyan" : "#56B6C2",
      "brightGreen" : "#98C379",
      "brightPurple" : "#C678DD",
      "brightRed" : "#E06C75",
      "brightWhite" : "#DCDFE4",
      "brightYellow" : "#E5C07B",
      "cyan" : "#56B6C2",
      "foreground" : "#DCDFE4",
      "green" : "#98C379",
      "name" : "One Half Dark",
      "purple" : "#C678DD",
      "red" : "#E06C75",
      "white" : "#DCDFE4",
      "yellow" : "#E5C07B"
    },
    "list": [
      {
        "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
        "name": "Windows PowerShell",
        "commandline": "powershell.exe",
        "hidden": false
      },
      {
        "guid": "{0caa0dad-35be-5f56-a8ff-afceeeaa6101}",
        "name": "命令提示符",
        "commandline": "cmd.exe",
        "hidden": false
      },
      {
        "guid": "{b453ae62-4e3d-5e58-b989-0a998ec441b8}",
        "hidden": false,
        "name": "Azure Cloud Shell",
        "source": "Windows.Terminal.Azure"
      },
      {
          "guid": "{2c4de342-38b7-51cf-b940-2309a097f518}",
          "hidden": false,
          "name": "Ubuntu",
          "source": "Windows.Terminal.Wsl"
      }
    ]
  },

  "schemes": [],

  "actions": [
    {
      "command": {
        "action": "copy",
        "singleLine": false
      },
      "keys": "ctrl+c"
    },
    {
      "command": "paste",
      "keys": "ctrl+v"
    },

    {
      "command": "find",
      "keys": "ctrl+shift+f"
    },

    {
      "command": {
        "action": "splitPane",
        "split": "auto",
        "splitMode": "duplicate"
      },
      "keys": "alt+shift+d"
    }
  ]
}

```