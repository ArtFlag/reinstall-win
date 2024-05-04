# reinstall-win

## Install apps

1. Start PowerShell as admin and install [Chocolatey](https://chocolatey.org/install). Run:

   ```powershell
   Set-ExecutionPolicy AllSigned
   Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
   ```

1. Install the apps:

   ```powershell
   choco install -y firefox `
   7zip hyper git vscode dropbox `
   skype signal telegram `
   discord steam-client epicgameslauncher origin `
   paint.net calibre sharpkeys k-litecodecpackfull `
   spotify malwarebytes `
   FiraCode deluge nordvpn geforce-experience
   ```

1. Install [MusicBee](https://getmusicbee.com/downloads/).
1. Install [Workman layout](https://github.com/workman-layout/Workman/zipball/master)
1. Use sharpkeys to map caps lock to ctrl.