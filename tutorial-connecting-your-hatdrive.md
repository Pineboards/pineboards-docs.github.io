### Connecting your HatDrive!

<img src="/assets/hatdrive-retail-packaging.jpeg" alt="logo" style="width: 100%"/>

#### Installing the hardware

Each HatDrive comes with the ribbon cable and the mounting hardware.

<img src="/assets/hatdrive-packaging-contents.jpeg" alt="logo" style="width: 100%"/>

There is an alignment triangle on both the ribbon and the HatDrive!, please use it to determine the right direction for inserting the cable.

<img src="/assets/hatdrive-top-with-nvme.jpeg" alt="logo" style="width: 100%"/>

#### Updating your Pi

The boards we currently ship to customers support HAT+ power management for PCIe devices. If the power LED on your Pineberry Pi board does not light up when you connect it for the first time you need to update your firmware. Execute following commands in your Raspberry Pi OS terminal:

`sudo apt-get update && sudo apt-get upgrade`

#### Enabling NVMe

If you do not intend to use your NVMe drive as a boot drive you need to enable the external PCIe port on the Pi 5:

Edit the boot config file (`sudo nano /boot/config.txt`)

Add `dtparam=nvme` to the bottom of the file, save it, and reboot

PCIe Gen 3 can be enabled with an additional config entry:

`dtparam=pciex1_gen=3`

#### Booting from NVMe

Boot order change is required to boot from NVMe. [Click here for more details](/tutorial-booting-from-nvme)
