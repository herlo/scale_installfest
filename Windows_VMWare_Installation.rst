Installing Fedora using VMWare Player
=====================================

Windows 10
~~~~~~~~~~
..
   Created: Fri, March 8, 2019
   Author: Clint Savage <herlo@socallinuxexpo.org>

This document covers how to install VMWare Player on Windows 10, which in turn, is used to install Fedora as a virtual machine.

Downloading VMWare Workstation Player
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Download the VMWare Workstation Player at

http://www.vmware.com/products/workstation-player/workstation-player-evaluation.html

.. image:: 01-download-vmware.png
   :scale: 85 %

Installing VMWare
~~~~~~~~~~~~~~~~~

Locate and double-click on the downloaded file. It should launch the installer.

.. image:: 02-install-vmware.png
   :scale: 85 %

follow the prompts as given below:

.. image:: 03-install-vmware.png

.. image:: 04-install-vmware.png

.. image:: 05-install-vmware.png

.. image:: 06-install-vmware.png

.. image:: 07-install-vmware.png

.. image:: 08-install-vmware.png


Restart
-------

After the last step (above), the computer will need to be restarted.

Launch VMWare
~~~~~~~~~~~~~

Upon reboot, there should be an icon on the desktop labeled 'VMWare Worksation Player 15' (or similar). Double-click the icon to start VMWare.

.. image:: 09-run-vmware.png
   :scale: 75 %

.. image:: 10-run-vmware.png
   :scale: 75 %

Create a New Virtual Machine (VM)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The VMWare Workstation 15 Player main screen should be displayed.

.. image:: 11-vmware-main-screen.png
   :scale: 85 %

Click 'Create a New Virtual Machine'

.. image:: 12-vmware-new-vm.png
   :scale: 85 %

Select the Fedora installation ISO.

.. note:: Use `Fedora-Workstation-netinst-x86_64-29-1.2.iso` from the provided labeled `ISOS` or `ISOS NTFS`.

.. todo:: Missing step 13

Choose `Linux` for the Guest Operating System

.. image:: 14-vmware-pick-os.png
   :scale: 85 %

Give the VM a Name. Use 'Fedora' or similar.

.. image:: 15-vmware-vm-name.png
   :scale: 85 %

Create a 20GB virtual disk for the operating system.

.. image:: 16-vmware-hard-disk.png
   :scale: 85 %

.. note:: Use 'Store virtual disk as a single file'

Click 'Finish' to create the VM.

.. image:: 17-vmware-confirm.png
   :scale: 85 %

Once the VM is created, it will be listed on the main screen

.. image:: 18-vmware-created.png
   :scale: 85 %

Start the Virtual Machine (VM)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Ensure the proper VM is selected, and choose `Play Virtual Machine`. If everything worked, the machine should begin to boot.

.. image:: 19-vmware-booting.png
   :scale: 85 %

Once the `vmware` boot screen comes up, the installer should start.

.. image:: 20-vmware-installer-booting.png
   :scale: 85 %

.. image:: 21-vmware-starting-installer.png
   :scale: 85 %

.. include:: install.rst

.. include:: bootintofedora.rst
