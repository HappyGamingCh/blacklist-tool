# TFT Blacklist Tool

http://blacklist.tool.tftrove.com

A Path of Exile 3rd Party Tool to warn you when you engage with a TFT Blacklisted User.

![blacklist tool showcase](/readme/blacklist-tool.gif)

![blacklist tool showcase](/readme/blacklist-tool.png)

## Download

Click [here](https://github.com/The-Forbidden-Trove/blacklist-tool/releases) to download.

Currently available in Windows

1. Unzip the zip file
2. Run `TFT Blacklist.exe`
3. Setup client log filepath via Settings Page (right click Icon -> Settings) if necessary.
    - It will try to search for `Client.txt` via default installation path, and if it doesn't exist, you may have to setup manually
    - The file is located in your game installation path, in the logs folder
    - Restart the app for the settings to take effect

## Feedback and Reports

For bug reports and general feedback please use the `#💬tool-dev-chat` ([link](https://discord.com/channels/645607528297922560/680796887259021342)) in our Discord Server

## Local blacklist entries

The application will also load names from a local blacklist file so you can add additional accounts that are not in the shared community list. By default the configuration points to [`local-blacklist.txt`](./local-blacklist.txt) in the root of the application folder (see the `BLACKLIST_FILE_PATH` field in [`config.json`](./config.json)). Add one character name per line and restart the tool to pick up the changes. The file ships with an example entry `ANATCHA2540#9419` that you can keep or replace with your own names.

## Building a Windows executable

If you would like to build the tool yourself, you can produce the Windows `.exe` bundle with the following steps:

1. Install dependencies with `npm install` (Electron 13 and `electron-packager` are required).
2. Run `npm run build` to package the Windows version. This writes the build to `dist/TFT Blacklist-win32-x64/` and produces `TFT Blacklist.exe` inside that directory.

The command works on Windows out of the box. When running on Linux or macOS you also need [`wine`](https://www.winehq.org/) available on your `PATH` so that `electron-packager` can set the application icon while creating the executable.

## Join Our Discord

[http://discord.tftrove.com](http://discord.tftrove.com)
