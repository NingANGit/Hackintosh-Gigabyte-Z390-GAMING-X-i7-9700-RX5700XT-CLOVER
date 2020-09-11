# Hackintosh

## Installation Windows en UEFI
https://www.youtube.com/watch?v=TyUnEP90e6o

## Installation MacOS
- Utiliser BalenaEtcher pour créer un bootable clé et graver le fichier d'installation OS dedans
- Monter EFI de la clé 
```
➜  ~ diskutil list
/dev/disk0 (internal, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      GUID_partition_scheme                        *500.3 GB   disk0
   1:                        EFI EFI                     314.6 MB   disk0s1
   2:                 Apple_APFS Container disk1         451.0 GB   disk0s2
   3:       Microsoft Basic Data BOOTCAMP                49.0 GB    disk0s3

/dev/disk1 (synthesized):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      APFS Container Scheme -                      +451.0 GB   disk1
                                 Physical Store disk0s2
   1:                APFS Volume Macintosh HD            11.3 GB    disk1s1
   2:                APFS Volume Macintosh HD - Data     132.2 GB   disk1s2
   3:                APFS Volume Preboot                 85.7 MB    disk1s3
   4:                APFS Volume Recovery                528.9 MB   disk1s4
   5:                APFS Volume VM                      4.3 GB     disk1s5

/dev/disk2 (external, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      GUID_partition_scheme                        *500.1 GB   disk2
   1:                        EFI EFI                     209.7 MB   disk2s1
   2:       Microsoft Basic Data WEPE                    524.3 MB   disk2s2
   3:                  Apple_HFS Install macOS Catalina  8.9 GB     disk2s3
   
➜  ~ sudo diskutil mount disk2s1
Password:
Volume EFI on disk2s1 mounted
```
- Remplacer les dossier booter & clover par ceux qui sont dans ce rép
- Rédémarrer & installation OS
## Installation MacOS
## Copie
Supprimer Boot de EFI du disk et replamcer par cceluieux qui sont dans usb
ccopier clover 
Microsoft Boot Clover
https://youtu.be/4lpDQzQ6iF0?t=1129
