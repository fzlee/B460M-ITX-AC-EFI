## Hackintosh for Asrock B460m ITX/AC. Big Sur supported

## 2024-06-22

Opencore 1.0.0
EFI for Sonoma 14.5

# Thanks to:

RapidEFI

@chenwutong

![](https://raw.githubusercontent.com/fzlee/B460M-ITX-AC-EFI/master/images/sonoma-14.5.png)

### Specs

- Asrock B460m ITRX/AC
- Intel 10500 with UHD630
- Kinstom HyperX 3200MHZ 16GB \* 2
- Intel 760P 512G SSD M.2
- BCM94352Z

### What Works:

1. Bluetooth, wireless, Airdrop.
2. DP and HDMI.
3. CPU/FAN sensors etc.
4. iCloud, iMessage etc.
5. Audio
6. Wake-On-Lan

### Notice

1. `device-id` is a must for DeviceProperties->PciRoot(0x0)/Pci(0x2,0x0), or you may suffer crashes on firefox, Photos etc.
2. DeviceProperties->PciRoot(0x0)/Pci(0x2,0x0)->framebuffer-stolenmem must be removed for iGPU or you may suffer resolution issue with 4K display
3. Serial number has been removed from PlatForm->Generic, you shoule generate with GenSMBIOS by yourself.
4. In some cases, onboard GPU doesn't work well with DP 4K display(boot into black screen), you can try to use HDMI instead. or try a discrete GPU.

### Post install

Sonoma has dropped support for Boroadcom wifi card, you need to enbale it with the following guide  
https://www.youtube.com/watch?v=gHs2CFox6gc&t=115s
