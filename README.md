# Ubuntu 18.04 - Bluetooth bug fix for kernel patch 4.15.x or later
Ubuntu 4.15 bluetooth source code patched with https://bugzilla.opensuse.org/attachment.cgi?id=770190

Bluetooth: hci0: don't support firmware rome 0x11020000 

Should fix Ubuntu Bug https://bugs.launchpad.net/ubuntu/+source/linux/+bug/1764645

To use : FOLLOW THE STEPS GIVEN BELOW:

--> sudo apt install git build-essential dkms

--> git clone https://github.com/anidaniel/ubuntu-btfix-4.15.git

--> sudo dkms add ./newbtfix-4.15

--> sudo dkms install btusb/4.0

--> Reboot
