# Enable wifi support with Qualcomm Atheros QCA6174

Enable the following:

```
CONFIG_MODULES=y
CONFIG_NET_VENDOR_ATHEROS=y
CONFIG_ATH_COMMON=y
CONFIG_WLAN_VENDOR_ATH=y
CONFIG_ATH10K=m
CONFIG_ATH10K_PCI=m
```

Download working firmware:

```
wget -O /lib/firmware/ath10k/QCA6174/hw3.0/firmware-4.bin "https://github.com/FireWalkerX/ath10k-firmware/blob/7e56cbb94182a2fdab110cf5bfeded8fd1d44d30/QCA6174/hw3.0/firmware-4.bin_WLAN.RM.2.0-00180-QCARMSWPZ-1?raw=true
wget -O /lib/firmware/ath10k/QCA6174/hw3.0/board.bin "https://github.com/FireWalkerX/ath10k-firmware/blob/7e56cbb94182a2fdab110cf5bfeded8fd1d44d30/QCA6174/hw3.0/board-2.bin?raw=true
```

Note: CONFIG_FIRMWARE_IN_KERNEL has no incidence regarding to how wifi works


## Tried, not working

```
MODULES=y
CONFIG_ATH10K=y
CONFIG_ATH10K_PCI=y
```

```
MODULES=y
CONFIG_ATH10K=y
CONFIG_ATH10K_PCI=y
```

```
MODULES=n
CONFIG_ATH10K=y
CONFIG_ATH10K_PCI=y
```

So, if ATH10K is not enabled *as a module*, it won't work
