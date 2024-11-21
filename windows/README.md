# Clean Installation of Windows 11

## Installation

1. Download a genuine Windows 11 ISO (e.g. from [here](https://massgrave.dev/genuine-installation-media)).
2. Create a bootable USB with [Rufus](https://rufus.ie/en/).
3. Connect the USB to your device.
4. Turn on the device and press the key that brings up the boot device menu.
5. Select the option to boot from the USB drive.
   - For the time and currency format, choose `English (World)`. This makes sure crap like TikTok don't get installed.
6. That's all.

## Activate Windows

1. Launch Powershell as administrator. Copy and paste the code below and press enter

   ```shell
   irm https://get.activated.win | iex
   ```

2. You will see the activation options. Choose `[1] HWID for Windows activation`.
3. That's all.

## Debloat Windows

1. Launch PowerShell as administrator. Copy and paste the code below and press enter

   ```shell
   irm "https://christitus.com/win" | iex
   ```

2. That's all.

## Restore the Old Right-click Context Menu

1. Open Registry Editor.
2. Navigate to the following address

   ```
   HKEY_CURRENT_USER\Software\Classes\CLSID
   ```

3. To create a new key, right-click the `CLSID` key in the left panel and select the `New > Key` option. A new key will be created.
4. Right-click the newly created key, select the `Rename` option and name it

   ```
   {86CA1AA0-34AA-4E8B-A509-50C905BAE2A2}
   ```

5. Then, create a sub-key under the above key that you just created. Name the key `InprocServer32`.
6. In the right panel, double-click the `Default` key, then close it without making any changes by clicking `OK`. This will make the value entry for it blank instead of `(value not set)`.
7. Close Registry Editor.
8. Restart Windows.
9. That's all.

## Essential Applications

- 7-Zip
- Aegisub
- Bulk Rename Utility
- Discord
- Firefox
- Google Drive
- HexChat
- HTTrack
- Icaros
- Logi Options+
- MediaInfo
- mpv
- MKVToolNix
- Mullvad VPN
- Obsidian
- PowerToys
- qBittorrent
- SumatraPDF
- Telegram
- Thunderbird
- Ungoogled Chromium
- Visual Studio Code
- Windows Subsystem for Linux (WSL)
- Windows Terminal
- Zoom
