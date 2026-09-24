Fedora build and corresponding boot partition image for Xiaomi Mi 8 Pro (equuleus)

Many thanks to https://github.com/redyuan43/xiaomi_8 for providing the boot image, DTB, and kernel for the equuleus device. 
I modified the mounting logic to use UUID="5ca4e0e7-a36d-4cb9-ad2f-f880c1d2bfc1" as the root partition and switch to it to launch the Fedora user space via systemd. 
You can connect to the Fedora instance running on the equuleus via SSH (using `ssh root@192.168.240.100`) through the virtual Ethernet interface that appears when connected to the host Linux distribution (please ensure no other network device on the LAN is using this IP address); the default password is `admin`.

