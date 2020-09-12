[WIP]
# Hackintosh-Gigabyte-Z390-GAMING-X-i7-9700-RX5700XT
Procedure and some source file including EFI used when I install hackintosh Catalina 10.15.6

## Configuration

| Hardware            | Article                                                        | Amazon Link                                 |
|---------------------|----------------------------------------------------------------|---------------------------------------------|
| Montherboard        | Gigabyte Z390 Gaming X                                         | https://www.amazon.fr/gp/product/B07HS4XS93 |
| CPU                 | Processeur Intel Core i79700                                   | https://www.amazon.fr/gp/product/B07S1MWTQ3 |
| Graphic Card        | SAPPHIRE Nitro+ Radeon RX 5700 XT 8G GDDR6                     | https://www.amazon.fr/gp/product/B07XGV3FL3 |
| RAM                 | HyperX Predator HX432C16PB3A/83200 MHz DDR4 CL16 DIMM XMP 8 GB | https://www.amazon.fr/gp/product/B07GLNMS1M |
| Solid State Drives  | Samsung SSD Interne 970 EVO Plus NVMe M.2 (500 Go)             | https://www.amazon.fr/gp/product/B07MFBLN7K |
| Wifi&Bluetooth Card | Broco Bluetooth 4.1 1300Mbps                                   | https://www.amazon.fr/gp/product/B081F8ZC38 |

## Install Windows with UEFI
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
