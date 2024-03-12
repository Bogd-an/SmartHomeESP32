
## Встановлення wsl та додавання usbUart

[туторіал](https://learn.microsoft.com/ru-ru/windows/wsl/connect-usb)


---

Встановити [usbipd msi](https://github.com/dorssel/usbipd-win/releases)

PowerShall в режимі адміна
```
usbipd list
usbipd bind --busid СВІЙ_BUSID
usbipd attach --wsl --busid СВІЙ_BUSID
```

В WSL
```
lsusb
ls /dev/ttyUSB*
```



В мому випадку
```
usbipd attach --wsl --busid 3-1
```