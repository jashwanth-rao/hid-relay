# USB HID Relay Control

## Linux
No additional program needed to use the usb HID relay from Linux.

---
Command to find the last connected hidraw device
```
ls $(find /sys/devices -iname '*:5131:2007.*')/hidraw
```

---
### Relay Switch 1:
Command to turn on:
```
echo -e '\xA0\x01\01\xA2' > /dev/hidraw1
```
Command to turn off:
```
echo -e '\xA0\x01\00\xA1' > /dev/hidraw1
```

---
### Relay Switch 2:
Command to turn on:
```
echo -e '\xA0\x02\01\xA3' > /dev/hidraw1
```
Command to turn off:
```
echo -e '\xA0\x02\00\xA2' > /dev/hidraw1
```

---
### Relay Switch 3:
Command to turn on:
```
echo -e '\xA0\x03\01\xA4' > /dev/hidraw1
```
Command to turn off:
```
echo -e '\xA0\x03\00\xA3' > /dev/hidraw1
```

---
### Relay Switch 4:
Command to turn on:
```
echo -e '\xA0\x04\01\xA5' > /dev/hidraw1
```
Command to turn off:
```
echo -e '\xA0\x04\00\xA4' > /dev/hidraw1
```
