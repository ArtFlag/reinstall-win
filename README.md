# reinstall-win

## Install apps

1. Start PowerShell as admin and install [Chocolatey](https://chocolatey.org/install). Run:

   ```powershell
   Set-ExecutionPolicy AllSigned
   Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
   ```

1. Download [config.json](./config.json) to `~/Downloads`.
1. Use [WinUtil](https://github.com/ChrisTitusTech/winutil) to reinstall apps.
   In an admin PowerShell prompt:

   ```powershell
   iex "& { $(irm christitus.com/win) } -Config ~/Downloads/config.json -Run"
   ```

   > **Note:** To run it manually:
   >
   > ```powershell
   > irm https://christitus.com/win | iex
   > ```

1. Install remaining apps:

   ```powershell
   choco install -y `
   dropbox calibre sharpkeys spotify workman`
   FiraCode nordvpn geforce-experience
   ```

   > **Note:**
   > If the workman package fails, use the [installer](https://github.com/workman-layout/Workman/zipball/master).

1. Use sharpkeys to map caps lock to ctrl.