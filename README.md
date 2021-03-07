# reinstall-win

## Install drivers

- [Drivers](https://www.gigabyte.com/Motherboard/GA-Z77-D3H-rev-10/support#support-dl-driver-audio)
  for Gigabyte Technology Co., Ltd. Z77-D3H rev 1.0.

## Install apps

1. Start PowerShell as admin and install [Chocolatey](https://chocolatey.org/install). Run:

   ```powershell
   Set-ExecutionPolicy AllSigned
   Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
   ```

1. Install the apps:

   ```powershell
   choco install -y directoryopus firefox brave `
   7zip hyper python3 git vscode dropbox `
   skype whatsapp discord steam uplay epicgameslauncher origin `
   paint.net calibre sharpkeys k-litecodecpackfull `
   musicbee spotify bleachbit malwarebytes jdownloader `
   FiraCode deluge authy-desktop
   ```
