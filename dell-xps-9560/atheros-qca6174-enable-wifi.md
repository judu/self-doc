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

Install linux-firmware:

```
cave resolve -zx linux-firmware
```

(Or, if you are not on exherbo, get it from https://git.kernel.org/cgit/linux/kernel/git/firmware/linux-firmware.git/ )

Note: You *have to* enable module support *and* make `ATH10K` and `ATH10K_PCI` modules.
Note 2: `CONFIG_FIRMWARE_IN_KERNEL` has no incidence regarding to how wifi works


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
