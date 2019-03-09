Installing Fedora using VirtualBox
=====================================

Mac OSX
~~~~~~~
..
   Created: Fri, March 8, 2019
   Author: Clint Savage <herlo@socallinuxexpo.org>
           Trevor Sharpe <tsharpe@gmail.com>

This document covers how to install VirtualBox on Mac OSX. Which in turn, is used to install Fedora as a virtual machine.

Obtaining VirtualBox Player
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Obtain a USB from a proctor labeled ISOS, and copy everything to your computer.

The VirtualBox-6.0.4-128413-OSX.dmg should specifically be copied, along with any ISOs.

Alternative Downloads
---------------------

Download VirtualBox-6.0.4-128413-OSX.dmg at

http://192.168.0.254/cblr/ISOs/VirtualBox-6.0.4-128413-OSX.dmg

If all else fails, download the VirtualBox Player at

https://download.virtualbox.org/virtualbox/6.0.4/VirtualBox-6.0.4-128413-OSX.dmg

.. image:: macosx_vbox/01-download-vbox.png
   :scale: 85 %

Installing VirtualBox
~~~~~~~~~~~~~~~~~~~~~

Locate and double-click on the downloaded file. It should launch the installer.

.. image:: macosx_vbox/02-install-vbox.png

follow the prompts as given below:

.. image:: macosx_vbox/03-install-warn.png

.. image:: macosx_vbox/04-install-progress.png

.. image:: macosx_vbox/05-install-success.png


Launch VirtualBox
~~~~~~~~~~~~~~~~~

Find VirtualBox and double-click the icon.

.. image:: macosx_vbox/06-vbox-main.png

The VirtualBox main screen should be displayed.

Create a New Virtual Machine (VM)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Select 'New' from the main screen and fill in the blanks.

.. image:: macosx_vbox/07-vbox-new-vm.png

Create a virtual disk for the operating system.

.. image:: macosx_vbox/08-vbox-hard-disk.png

.. image:: macosx_vbox/09-vbox-hdd-file-type.png

.. image:: macosx_vbox/10-vbox-hdd-storage-type.png

Create a large enough hard drive (20GB is safe)

.. image:: macosx_vbox/11-vbox-hdd-size.png

A VM should successfully be created at this point.

.. image:: macosx_vbox/12-vbox-vm-created.png

The VM needs a CD attached. Choose `Settings`.

.. image:: macosx_vbox/13-vbox-vm-settings.png

Choose `Storage`, then `Controller: SATA`. Click the CD and plus icon.

.. image:: macosx_vbox/15-vbox-vm-storage-sata.png

Choose the Add button along the top.

.. image:: macosx_vbox/16-vbox-vm-storage-add.png

Select the Fedora installation ISO file.

.. image:: macosx_vbox/17-vbox-vm-storage-fedora-live.png

.. note:: Use `Fedora-Workstation-Live-x86_64-29-1.2.iso` from the provided labeled `ISOS` or `ISOS NTFS`.

Start the Virtual Machine (VM)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Select `Start` from the Main Menu with the appropriate VM selected.

.. image:: macosx_vbox/12-vbox-vm-created.png

Upon boot, a menu will appear prompting for a selection.

Select `Test this media & Start ...`

.. image:: macosx_vbox/18-vbox-boot-f29-live.png

After booting, the Fedora Desktop should appear with options to 'Try Fedora' or 'Install to Hard Drive'.

Select 'Install to Hard Drive'

.. image:: macosx_vbox/19-vbox-f29-desktop.png

.. include:: install.rst

.. include:: bootintofedora.rst
