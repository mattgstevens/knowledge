# Recover data from an encrypted LUKS volume

- create a new live boot USB from an iso
- start with live boot image
- `sudo fdisk -l` -> see what device is the encrypted drive
- `sudo cryptsetup luksOpen /dev/{device} data` -> enter password to unlock LUKS and open
- `sudo mkdir /mnt/data` -> prepare a mount directory
- `sudo mount /dev/mapper/data /mnt/data` -> mount the unlocked LUKS volume

You can now see your encrypted data at `/mnt/data`
