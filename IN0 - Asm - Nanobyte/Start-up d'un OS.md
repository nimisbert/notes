Souvent une phase prise en charge par un BIOS/Bootloader.
## Legacy booting
- Le BIOS cherche le premiers secteur bootable d'un device en mémoire 0x7C00
- Le BIOS vérifie la présence d'une signature 0xAA55
- Si le secteur de Boot contient la signature, le code du secteur est exécuté
## EFI booting
- Le BIOS cherche des partitions EFI 
- L'OS doit être compiler en tant qu'EFI