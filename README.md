## Hackintosh for Asrock B460m ITX/AC

EFI for catalina 10.15.6

![](https://raw.githubusercontent.com/fzlee/B460M-ITX-AC-EFI/master/images/catalina-10.15.6.png)

### specs
Asrock B460m ITRX/AC
Intel 10500 with UHD630
Kinstom HyperX 3200MHZ 16GB * 2
Intel 760P 512G SSD M.2
BCM94352ZQ


### What Works:
1. Bluetooth, wireless, Airdrop.
2. DP and HDMI.
3. CPU/FAN sensors etc.
4. icloud, iMessage etc.

### What broken:
Audio


### Notice

1. `device-id` is a must for DeviceProperties->PciRoot(0x0)/Pci(0x2,0x0), or you may suffer crashes on firefox, Photos etc. 
2. Serial number has been removed from PlatForm->Generic, you shoule generate with SMBIOS by yourself.

