# find-grub-after-win-updates

Updates of windows on 6th June 2022 made my ubuntu grub dispear. 

Lap: Lenevo xiaoxin 13 pro. Dual boot of windows 11 & ubuntu 18.04.6 (5.4.109 & 110)

Problem: 
I cant boot into Ubuntu as there's no grub.
Easyufei shows windows always keeps the priority.

Solution on windows: 
1. DiskInternals Linux Reader - copy files from Ubuntu
2. Run cmd as administrator: bcdedit /set {bootmgr} path \EFI\ubuntu\shimx64.efi (grubx64.efi doesn't work)

Failed attampts: 
ubuntu live & boot-repair cant work without wifi. Lap has trouble in wifi drive on most kernels. Hate that.
