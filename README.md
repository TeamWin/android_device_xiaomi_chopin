# TWRP Device Configuration for Poco X3 Gt/Redmi Note 10 Pro 5G

The Poco X3 Gt/Redmi Note 10 Pro 5G (codenamed _"chopin"_) is a high-end, mid-range smartphone from Xiaomi.
It was released in May 2021.

## Device specifications

| Basic                   | Spec Sheet                                                                                                                     |
| -----------------------:|:------------------------------------------------------------------------------------------------------------------------------ |
| CPU                     | Octa-core                                                                                                                      |
| Chipset                 | Mediatek Dimensity 1100                                                                                                        |
| GPU                     | Mali-G77 MC9                                                                                                                   |
| Memory                  | 6/8 GB RAM                                                                                                                     |
| Shipped Android Version | 11.0                                                                                                                           |
| Storage                 | 128/256 GB                                                                                                                     |
| Battery                 | Non-removable Li-Po 5000 mAh battery                                                                                           |
| Display                 | 1080 x 2400 pixels, 20:9 ratio (~399 ppi density),60/120 Hz                                                                    |
| Camera (Back)(Main)     | 64 MP, f/1.8, 26mm (wide), 1/1.97", 0.7µm, PDAF                                                                                |
| Camera (Front)          | 16 MP, f/2.5, (wide), 1/3.06", 1.0µm                                                                                           |

## Device picture

![Redmi Note 10 Pro/POCO X3 GT](https://cdn.cnbj0.fds.api.mi-img.com/b2c-shopapi-pms/pms_1621955784.84614979.jpg "Redmi Note 10 Pro/POCO X3 GT")

# Status
Current state of features (from [here](https://twrp.me/faq/OfficialMaintainer.html)):

### Blocking checks
- [ √ ] Correct screen/recovery size
- [ √ ] Working Touch, screen
- [ √ ] Backup to internal/microSD
- [ √ ] Restore from internal/microSD
- [ √ ] reboot to system
- [ √ ] ADB

### Medium checks
- [ √ ] update.zip sideload
- [ √ ] UI colors (red/blue inversions)
- [ √ ] Screen goes off and on
- [ √ ] F2FS/EXT4 Support, exFAT/NTFS where supported
- [ √ ] all important partitions listed in mount/backup lists
- [ √ ] backup/restore to/from external (USB-OTG) storage (not supported by the device)
- [ √ ] backup/restore to/from adb (https://gerrit.omnirom.org/#/c/15943/)
- [ √ ] decrypt /data
- [ √ ] Correct date

### Minor checks
- [ √ ] MTP export
- [ √ ] reboot to bootloader
- [ √ ] reboot to recovery
- [ √ ] poweroff
- [ √ ] battery level
- [ √ ] temperature
- [ √ ] encrypted backups
- [ √ ] input devices via USB (USB-OTG) - keyboard, mouse and disks (not supported by the device)
- [ × ] USB mass storage export
- [ √ ] set brightness
- [ × ] vibrate
- [ √ ] screenshot
- [ × ] partition SD card


# Building
```bash
source build/envsetup.sh
lunch twrp_chopin-eng
mka bootimage -j$(nproc --all)
```

# Flashing
Follow [this](https://twrp.me/faq/OfficialMaintainer.html) guide.
