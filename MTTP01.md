# Mass Deletion
## Platform: Linux / Mac / Mobile / Windows

## Permissions Required: Non Admin (Admin for sensitive files)
## ID: MTTD01

### The intentional deletion of critical files or the unauthorized wiping of devices can have severe consequences for business operations, causing financial loss, reputational damage, and operational delays. Insiders with knowledge of sensitive data locations or device management systems can exploit their access to maliciously delete files, wipe devices, or disrupt business continuity. Monitoring and mitigating these activities is essential to protect company assets.

[Proof of concept script - Linux](https://github.com/djrk01/windowsattackstuff/blob/main/oops.sh)
<br>
<br>
https://github.com/KhalsaAnonymous/Bulk-File-Deleter
<br>
<br>
https://github.com/8/MFilesDeleter


Detection:

Tools:

•  Eraser — scheduled and on-demand secure file overwriting, multiple DoD/Gutmann pass options 

•  SDelete (Sysinternals) — Microsoft-signed CLI secure delete, commonly abused by insiders 

•  Cipher /w — built-in Windows command that overwrites free space to prevent carving 

•  DBAN (Darik's Boot and Nuke) — full disk wipe, used for drive destruction before offboarding 

•  Nwipe — Linux/live boot secure wipe utility, fork of DBAN 

•  Secure Empty Trash (macOS) — legacy macOS overwrite-on-delete feature 

•  FileShredder — GUI-based multi-pass file shredder for Windows 

•  Freeraser — portable Windows shredder with drag-and-drop interface

Built-in OS utilities 9. del /f /q (Windows CMD) — force-quiet deletion, 

bypasses recycle bin 10. rm -rf (Linux/macOS) — recursive force delete, no recovery prompt 11. 

shred (Linux) — overwrites file data before unlinking, defeats simple carving 12. wipe (Linux) — secure unlink with multiple overwrite passes

Privacy / anti-forensic suites

BleachBit — open-source privacy cleaner, clears logs, temp files, browser artifacts, and free space

PrivaZer — deep artifact cleaner targeting MFT entries, USN journal, prefetch, and shell history

MrClean — lightweight artifact and file remnant cleaner

CCleaner — widely used artifact cleaner, covers recycle bin, browser cache, temp files, and registry traces
