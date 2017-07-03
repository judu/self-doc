# Use Realtek card reader RTS525A

## lspci

```
03:00.0 Unassigned class [ff00]: Realtek Semiconductor Co., Ltd. RTS525A PCI Express Card Reader [10ec:525a] (rev 01)
        Subsystem: Dell RTS525A PCI Express Card Reader [1028:07be]
        Kernel driver in use: rtsx_pci
```

## Kernel modules

```
MMC=y
MMC_BLOCK=y
PCI_MMCONFIG=y
MMC_SDHCI=y                                                  
MMC_SDHCI_PCI=y
MMC_REALTEK_PCI=y
MFD_RTSX_PCI=y
```

And it should work out of the box.
