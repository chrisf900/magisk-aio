# Magisk-AIO (in process)

-Available in Taringa- 

Universal Systemless Compatibility

# Instructions:

Recommended: Restore back to 100% stock system + boot.

Minimal Requirement:
Remove ANY kind of root (SuperSU, phh's su, KingRoot...) 

Remove v85.x topjohnwu's Systemless Xposed, romracer's Systemless Xposed, official system Xposed by reverting to stock boot image or use uninstallers.

Please make sure to remove included root COMPLETELY (/system/xbin/su, /data/su.img, /sbin/su etc.)

Installer will patch system verity and forceencrpyt. If you want them not to be patched, configure by:
Code:
-----
 Remove previous configs
rm /cache/.magisk /data/.magisk
Keep verity
echo "KEEPVERITY=true" >> /cache(or data)/.magisk
Keep forceencrypt
echo "KEEPFORCEENCRYPT=true" >> /cache(or data)/.magisk

(If you want to use custom kernels: restore to stock boot image -> flash custom kernel -> flash Magisk)
(Optional) Download Magisk Manager and install on your device. Please note that root access is required.


Uninstall Magisk:
-------------------
Download the Magisk uninstaller and flash it in custom recoveries. 
It can remove Magisk installs from v1 to the latest version.
For users that custom recoveries cannot access data, the uninstaller will still work, but it won't uninstall completely. 
To remove completely, manually restore stock boot image, and manually remove /data/magisk.img, /cache/magisk, /data/busybox
