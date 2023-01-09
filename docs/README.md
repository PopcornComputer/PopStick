<p align="center"><img src="https://docs.usbcomputer.com/images/banner.jpg" alt="PopStick USB Computer Device"></p>

# PopStick™
Introducing the _innovative_ PopStick™, a new computer in a USB stick form-factor.

## Purchase
**PopStick™** is available for purchase in our webstore: [https://shop.popcorncomputer.com/products/popstick][webstore]

## Getting Started

Things to know:<br>
If booting from Internal Flash, please note that it will take up to 1-2 minutes to boot. Once the PopStick™ is booted successfully, you will see one of the LEDs blinking in a heartbeat pattern.

By using the USB micro B connector and plugging a cable into your computer. You can have access to the serial terminal output of the processor. Use this terminal on first boot so that you can set the root password.

The factory software install of the PopStick™ contains two users.
1. User: root<br> Password: None (Blank, see below for details)
2. User: popcorn <br>Password: popcorn

Upon logging into for the first time with root and until you set a password for it. You will automatically be dropped into a command-line without being prompted for a password. You will not be able to SSH into PopStick™ with root until you set a password.

Once the device has successfully booted, PopStick™ should show on your computer as a "Popcorn Ethernet / Serial" composite device without the need to install a driver.

The Ethernet device will automatically issue an IP to your computer and will be available at the following IP: 192.168.81.1 or 192.168.82.1 depending on your computer's operating system.

If you use a web browser to go to one of these IPs, you will see a documentation page loaded. This page is hosted on the PopStick™ using a lighttpd instance.

Further, depending on your computer's OS. There will be a COM port or /dev/ttyACM0 or /dev/tty.usbserial-### that you can connect to using a serial terminal program. The baudrate for this serial port is 115200.



## Software
### Build a Custom Linux OS using Buildroot
Using Buildroot, a simple and easy-to-use tool, you can generate a custom Linux OS for your PopStick™ that includes only what you need. We have provided a PopStick™ Buildroot Environment that has everything you need to quickly configure and cross-compile your own custom Linux environment.

https://github.com/PopcornComputer/Popstick-buildroot/

### U-Boot Bootloader
https://github.com/PopcornComputer/Popstick-uboot/

### Linux Kernel Staging Environment
https://github.com/PopcornComputer/Popstick-linux/

## Hardware
You can find the schematic, design files and bill of materials (BOM) in the **PopStick-Hardware** repository.<br>
https://github.com/PopcornComputer/PopStick-Hardware

## Contact
For sales inquiries, please email: <a href="mailto:sales@source.parts">sales@source.parts</a>

For support, please email: <a href="mailto:support@source.parts">support@source.parts</a>

[webstore]: https://shop.popcorncomputer.com/products/popstick
[popstick-hardware-repo]: https://github.com/PopcornComputer/PopStick-Hardware
