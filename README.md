# CSR-Barrot-8041a02
Patch for CSR v5.0 Bluetooth Dongle detected as fake chip\
Tested on Linux Kernel v5.16.11

```
[stellarix ~]$ lsusb -s 2 -v

Bus 001 Device 002: ID 0a12:0001 Cambridge Silicon Radio, Ltd Bluetooth Dongle (HCI mode)
Couldn't open device, some information will be missing
Device Descriptor:
  bLength                18
  bDescriptorType         1
  bcdUSB               2.00
  bDeviceClass          224 Wireless
  bDeviceSubClass         1 Radio Frequency
  bDeviceProtocol         1 Bluetooth
  bMaxPacketSize0        64
  idVendor           0x0a12 Cambridge Silicon Radio, Ltd
  idProduct          0x0001 Bluetooth Dongle (HCI mode)
  bcdDevice           88.91
  iManufacturer           0 
  iProduct                2 BT DONGLE10
  iSerial                 0 
  bNumConfigurations      1
```

```
[    4.388800] Bluetooth: hci0: CSR: Unbranded CSR clone detected; adding workarounds and force-suspending once...
[    4.388805] Bluetooth: hci0: CSR: Failed to suspend the device for our Barrot 8041a02 receive-issue workaround
```
