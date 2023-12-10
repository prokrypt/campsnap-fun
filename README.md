# campsnap-fun
random stuff on the camp snap camera

## operation
* make sure camera is charged
* hold down shutter button
* display shows `---`. keep holding the button!
* device beeps after ~2.5 seconds and you can let go of the button
* wait another ~3 seconds for device to finish booting and scan the microsd card (for 148 photos in my case)
* display shows the amount of photos taken
* ready to take photos! press shutter button
* display shows `---`
* wait ~0.8 seconds until shutter sound plays, indicating the photo has been taken
* wait another ~2.5 seconds for it to save photo
* display shows amount of photos taken

## dmesg with stock microsd card
```
[0.120121] usb 5-1.1.3: new high-speed USB device number 78 using xhci_hcd
[0.272862] usb 5-1.1.3: New USB device found, idVendor=04fc, idProduct=1628, bcdDevice= 1.00
[0.272874] usb 5-1.1.3: New USB device strings: Mfr=1, Product=2, SerialNumber=0
[0.272880] usb 5-1.1.3: Product: General Image Device
[0.272885] usb 5-1.1.3: Manufacturer: Icatchtek Co Ltd 
[0.342199] usb 5-1.1.3: Found UVC 1.00 device General Image Device (04fc:1628)
[1.433795] usb 5-1.1.3: Failed to query (GET_INFO) UVC control 2 on unit 2: -71 (exp. 1).
[1.434138] usb 5-1.1.3: Failed to query (GET_INFO) UVC control 3 on unit 2: -71 (exp. 1).
[1.434518] usb 5-1.1.3: Failed to query (GET_INFO) UVC control 6 on unit 2: -71 (exp. 1).
[1.434873] usb 5-1.1.3: Failed to query (GET_INFO) UVC control 7 on unit 2: -71 (exp. 1).
[1.435241] usb 5-1.1.3: Failed to query (GET_INFO) UVC control 8 on unit 2: -71 (exp. 1).
[1.435616] usb 5-1.1.3: Failed to query (GET_INFO) UVC control 5 on unit 2: -71 (exp. 1).
[1.492286] usb 5-1.1.3: UVC non compliance - GET_DEF(PROBE) not supported. Enabling workaround.
[1.492656] uvcvideo 5-1.1.3:1.1: Failed to query (129) UVC probe control : -71 (exp. 26).
[1.492667] uvcvideo 5-1.1.3:1.1: Failed to initialize the device (-71).
[1.927458] usb 5-1.1.3: USB disconnect, device number 78
[2.197245] usb 5-1.1.3: new high-speed USB device number 79 using xhci_hcd
[2.345415] usb 5-1.1.3: New USB device found, idVendor=04fc, idProduct=0171, bcdDevice= 1.00
[2.345420] usb 5-1.1.3: New USB device strings: Mfr=1, Product=2, SerialNumber=3
[2.345422] usb 5-1.1.3: Product: General Image Device
[2.345423] usb 5-1.1.3: Manufacturer: Icatchtek Co Ltd 
[2.345425] usb 5-1.1.3: SerialNumber: 20100805 01.00
[2.388158] usb-storage 5-1.1.3:1.0: USB Mass Storage device detected
[2.388576] scsi host2: usb-storage 5-1.1.3:1.0
[3.411916] scsi 2:0:0:0: Direct-Access                General             PQ: 0 ANSI: 0 CCS
[3.414182] sd 2:0:0:0: [sdb] 7864320 512-byte logical blocks: (4.03 GB/3.75 GiB)
[3.415451] sd 2:0:0:0: [sdb] Write Protect is off
[3.415454] sd 2:0:0:0: [sdb] Mode Sense: 20 00 00 00
[3.416721] sd 2:0:0:0: [sdb] No Caching mode page found
[3.416724] sd 2:0:0:0: [sdb] Assuming drive cache: write through
[3.426180]  sdb: sdb1
[3.427153] sd 2:0:0:0: [sdb] Attached SCSI removable disk
```

more to come...
