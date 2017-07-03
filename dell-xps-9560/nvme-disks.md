# Enable NVMe for disks

```
CONFIG_NVME_CORE=y
CONFIG_BLK_DEV_NVME=y
CONFIG_BLK_DEV_NVME_SCSI=y
```

Note: not tried to disable `NVME_SCSI`.
