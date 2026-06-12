<img width="477" height="131" alt="Image" src="https://github.com/user-attachments/assets/408d9ef2-bb64-4be4-a6a8-7bbc5e855853" />

<!-- 
Upload images to GitHub

Create a new issue on GitHub.

Drag an image into the comment field.

Wait for the upload process to finish.

Copy the URL and use it in your Markdown files on GitHub.
 -->
# How to Install LastOSLinux
v1.0.0

**Things you will need:**

* A x64 Compatible PC/Laptop with 4GB+ of ram and 60GB+ HDD space.  
* A USB stick with 8GB+ or larger (USB 3 if available).  
* Access to BIOS to disable SecureBoot \*

\* SecureBoot \~ Linux generally doesn’t work well with SecureBoot so this should be disabled in your BIOS before attempting to install Linux or install and Drives while in Linux (It can be re-enabled once it’s installed, but it’s still not recommended). To disable SecureBoot you will need to boot to BIOS when you first turn the PC on, this is achieved by pressing a key on the keyboard, usually Esc, F1 to F12 or the Del key, find SecureBoot and change it to Disabled, many PC’s will ask you to type in 4 numbers to make this change.

**Where to get the LastOSLinux ISO:**

First visit [www.lastos.org/lastoslinux](http://www.lastos.org/lastoslinux) to read about this OS, feel free to click the LastOS icon on the sidebar to go to the forums where you can ask questions or get support, it may even have the answers you need in from other peoples questions.

On the page above in the Download ISO section is a Download Now button. Clicking this will open to a sourceforge link where it is hosted: [https://sourceforge.net/projects/lastoslinux/files/ISOs/](https://sourceforge.net/projects/lastoslinux/files/ISOs/) if you click the latest dated ISO you will be able to download the very latest public version of LastOSLinux to either burn to DVD or make a bootable USB to install from.

**Making a bootable USB:**

Before you can make a bootable USB you will need the above ISO and a USB stick or portable device that is 8GB or larger.

\* Note: All the data on the USB will be deleted so make sure you have any important files backed up if you need to keep any of them.

From Windows;  
If you are using windows the very best option to make a Bootable USB is to use the Rufus tool, you can also use Ventoy if you're more experienced in computers and understand that making a Ventoy USB can boot from any ISO file you copy to it. Watch a youtube video or google how to use Ventoy if you need to use this method.

Rufus Steps;

1. Download [https://rufus.ie/downloads/](https://rufus.ie/downloads/) latest portable version (rufus-4.7p.exe at the time of creating this document).  
2. Next place the 8GB+ USB into a fast USB slot in your computer (The blue ports or the ones that say SS on them are USB3 and could prepare the USB stick a lot faster than using a standard USB2 port if the USB Stick is also USB3 compatible.  
3. Run rufus-4.7p.exe  
4. In the top drop down combo box click the down arrow on the far right, then select the USB stick you have inserted (check the size matches and the brand/name is the same as shown in “This PC”, to make sure you have selected the correct one. By default it hides internal disks, but any USB can be selected to be erased so be careful).  
5. In the next “Boot selection” press the “SELECT” combo box, browse for the downloaded ISO from above “LastOSLinux\_amd64\_2025-03-22\_Public\_Final.iso”. This step may ask to download the syslinux boot files it needs to create a bootable USB, press Yes/Allow when asked.  
6. Change the “Partition scheme” to MBR if it is set to GPT (GPT can work, but MBR is more compatible and will work with more PC’s)  
7. Press Start and follow the warning/info prompts and allow it to complete building the bootable USB.

**Follow a video guide to making a Bootable USB:**  
[https://youtu.be/P4yjeVHYmSg](https://youtu.be/P4yjeVHYmSg)

**Follow a video for making a Ventoy Bootable USB:** (To do this in Windows you can download the windows version of Ventoy)  
[https://youtu.be/PHkgpoYOpsM?si=fX\_y8qdaAV7TTO0b](https://youtu.be/PHkgpoYOpsM?si=fX_y8qdaAV7TTO0b)

**Follow a Video Installation Guide:**  
[https://youtu.be/3U7ougYcCZs](https://youtu.be/3U7ougYcCZs)

**Booting from the USB stick:**

1. On the PC you want to install first turn it off and plug in the USB stick created above.  
2. Make sure SecureBoot has been disabled in your BIOS (LastOSLinux can not be installed while SecureBoot is enabled).  
3. When you first turn on the PC/Laptop start tapping Esc, F1 to F12 or the Del key to bring up the boot menu. It sometimes has which key to press to change the boot order, some people say just run your finger along all of them but this seems like it could boot the UEFI or BIOS instead of just the boot menu. If you do go into some BIOS’s it also allows you to pick the boot device one time, which can also work. If you still are unable to get it to boot, as a last resort you can change the boot order in BIOS to put the USB first, some older machines may fail to write the HDD boot file to the HDD and would make it unable to boot without the USB inserted (this doesn’t affect newer machines).  
4. When the boot menu shows pick “LastOSLinux LiveOS”, this is the OS you can start to check everything is working properly before you install the OS to your computer, it is also used to start the installer.

**LiveOS/Install:**

Once the LiveOS starts you should be on the desktop with an Icon “Install LastOSLinux”. Before you start this install, go to the Network/WiFi icon near the clock and log into your network so you have internet. Try adjusting the volume and listen if the sound is working. If you can see, hear and use the internet then you should be right to proceed with the installation.

1. Double click the “Install LastOSLinux” icon on the desktop, this may take a couple of minutes to begin.  
2. First check the Location is set correctly by clicking the map or manually selecting it from the named places.  
3. Pick the correct Keyboard layout for you, usually it will best guess the keyboard from the location \- which is incorrect when using Australia as your Location, we use the US keyboard layout so you will need to change from “English (Australian)” to “English (US)” before you press Next.  
4. Next is the partitioning of the internal HDD’s to where you will be installing the OS, this is custom for each person depending on your needs, explained below \*  
5. \* User / Owner \- would set the Name to the full owners name  
   \* Login Name \- usually the first name or first initial and last name or a nickname (all lowercase with no capital letters or spaces or special characters)  
   \* Computer/PC Name is shown on the Network (usually the first name with pc or a number written after it (do not use special characters or spaces)  
   \* Set a password for the user account (you can use a very simple password for home users if you do not have important documents and they are backed up separately off the computer, especially if you have enabled 2FA for any banking or important tasks), I generally set the password to “x” on my installs and let the user change them once they receive their PC back.  
     
   Press Next and a summary screen will be shown, confirm you are happy and proceed with the installation.  
   

\* To Partition your computer HDD (best practices);

Many people will often just pick Erase and use the whole HDD for their installation, this has the downside of making any future OS installations require you to backup any important settings and documents before you reinstall, it also means you are not able to properly run a “TimeShift” backup without extra work excluding it from being backed up as well. To make things easier I instead make the OS separate to the Home folder (Users Documents and Settings), allowing you to reinstall/restore/recover any Linux OS without having to backup/restore your files \- this does not mean you do not have to keep external backups, just that you won’t have to restore from your backups after a clean installed PC.

1. Pick Manual partitioning  
2. Check the disk it has selected up the top right is the correct disk for your OS  
3. If you are starting with a fresh configuration you are best to remove all partitions from the disk by pressing “New Partition Table”, if you are reinstalling you can just set the mount points from your previous Linux OS and make sure “Format” isn’t selected where you do not wish it to remove files from that partition.  
4. Starting from a fresh Partition Table (or picking existing partitions), Create and set the first partition to be 1.6GB (Change “File System” to “fat32”) then you need to tick the “boot” option from the flags list below it. The last step is you set the mount point to “/boot/efi”, this makes the UEFI work, if your PC is older (no UEFI) then just do NOT set a mount point at all in the boot partition\! It is enough to just set the “boot” Flag for it to be used.  
5. Create and set the next partition to be 60GB for a 128GB HDD, or 90GB if 256GB HDD or bigger, the OS will usually never grow to be above 40 or 50GB, but it doesn’t hurt to have a little space for it to do updates/upgrades etc, if you have even bigger disks you can make it 120GB to make it fully future proof. Set “File System” to “ext4” and change the Mount Point to “/” a single forward slash, this is the root of the main OS and if you do nothing else and use all of the HDD space left it will be the same as a “Erase” install not a “Custom” install. Do NOT pick any flags for this partition.  
6. As we want the Home / Users files off the main OS Partition we Create another partition with the remaining space, Change “File System” to “ext4” and set the Mount Point to “/home” (Make sure the Format option isn’t selected unless you want it to erase the user files already on that partition\!

Once your OS has successfully installed it will ask if you want to reboot, at this stage you can remove the USB from the PC and LastOSLinux will continue once it first boots to the desktop \- everything it needs is pre-copied off the USB during the initial setup.

LastOSLinux is designed to layer on top of the underlying Operating system base, this means it will be able to be upgraded the same as the Vanilla (original) OS, currently only Linux Mint is used for LastOSLinux ISO’s but in the future this will include Nobara, Fedora, BigLinux and others as I find the best methods to do so.

Linux Mint Base: [https://linuxmint.com/](https://linuxmint.com/)   
Upgrade Help: [https://linuxmint-user-guide.readthedocs.io/en/latest/upgrade.html](https://linuxmint-user-guide.readthedocs.io/en/latest/upgrade.html) 

**Run LLStore to install extra Apps and Games or apply tweaks:**

Running LLStore from the Desktop/Menu or the USB you are able to pick what you want to install extra to the OS, many of the items included will run on any Linux Distribution, the Windows based ones can be installed through Wine or even in Windows, I made LLStore fully portable and able to be ran on most OS's

[https://youtu.be/4xF1kvYtbv4](https://youtu.be/4xF1kvYtbv4)

**TimeShift Backups:**

You can use the included Tool named TimeShift to take incremental Images of your running OS to restore from the LiveOS, you can also hold shift as your PC tries to boot and access the Advanced \- Recovery environment to restore any of these images back over the top.

Watch Video of TimeShift capture and a restore:  
[https://youtu.be/-58j5eTapmY](https://youtu.be/-58j5eTapmY)  
