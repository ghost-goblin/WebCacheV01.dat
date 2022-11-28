```sh
schtasks /Change /TN "\Microsoft\Windows\Wininet\CacheTask" /Disable
schtasks /end /tn "\Microsoft\Windows\Wininet\CacheTask"
taskkill /im dllhost.exe /f
del "AppData\Local\Microsoft\Windows\WebCache\WebCacheV01.dat"
```
