## Hackintosh for Asrock B460m ITX/AC. Big Sur supported

Opencore 7.3
EFI for Big Sur 11.5.2

# Thanks to:
@chenwutong

![](https://raw.githubusercontent.com/fzlee/B460M-ITX-AC-EFI/master/bugsure.11.5.2.png)

### Specs

* Asrock B460m ITRX/AC
* Intel 10500 with UHD630
* Kinstom HyperX 3200MHZ 16GB * 2
* Intel 760P 512G SSD M.2
* BCM94352Z
* no dGPU 


### What Works:
1. Bluetooth, wireless, Airdrop.
2. DP and HDMI.
3. CPU/FAN sensors etc.
4. iCloud, iMessage etc.
5. Audio
6. Wake-On-Lan

### Notice

1. `device-id` is a must for DeviceProperties->PciRoot(0x0)/Pci(0x2,0x0), or you may suffer crashes on firefox, Photos etc. 
2. Serial number has been removed from PlatForm->Generic, you shoule generate with GenSMBIOS by yourself.

