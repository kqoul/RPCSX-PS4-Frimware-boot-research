#RPCSX PS4 Frimware boot research

Documenting my personal attempts into getting the PS4 firmware running on RPCSX

## current setup
- OS: NixOS 26.11 (Zokor) x86_64
- RPCSX ver: v20260630-e8ae148
- CPU: Ryzen 5 5600H
- GPU: Nvidia GTX 1650 Mobile 4GB VRAM
- RAM: 8GB

## Progress

### Frimware Version 7.00

- .PUP.dec Unpacked succesfully
- 'system_fs_image.img" mounted successfully
- RPCSX recognized the frimware file system and the attempt to boot
- Boot failed because RPCSX didnt find "mini-syscore.elf"

 Error:

	'Failed to open '/mini-syscore.elf''

## Frimware Version 5.00

- Same exact point where i got stuck on V7.00


### Current investigation

Trying to determine why, how, and where RPCSX expects 'mini-syscore.elf', and also trying to figure out what exact layout it expects

