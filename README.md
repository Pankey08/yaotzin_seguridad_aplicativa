# yaotzin_seguridad_aplicativa

echo Set obj = CreateObject("WScript.Shell") > C:\Users\XMK8875\AppData\Local\Temp\run.vbs
echo obj.Run "cmd.exe /k whoami" >> C:\Users\XMK8875\AppData\Local\Temp\run.vbs
cscript C:\Users\XMK8875\AppData\Local\Temp\run.vbs

wmic service get name,pathname,startmode | findstr /i "auto" | findstr /i /v "c:\windows\\" | findstr /i /v """"
