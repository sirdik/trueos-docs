.. index:: introduction
.. _Introducing TrueOS:

Introducing |trueos|
********************

Written by users of the |trueos| operating system.

Welcome to |trueos|!

This Handbook covers the installation and use of |trueos|. This Handbook
is a work in progress and relies on the contributions of many
individuals. To assist with the Handbook, refer to the documentation
`README <https://github.com/trueos/trueos-docs/blob/master/trueos-handbook/README.md>`_.
If using IRC Freenode, join the #trueos channel and converse with many
other |trueos| users. `Gitter <https://gitter.im/trueos>`_ is
another popular option for users.

`TrueOS® <http://www.trueos.org>`_ (formerly known as |pcbsd|) began in
2005 when Kris Moore presented the first beta version of a FreeBSD
operating system pre-configured for desktop use. Since then, |trueos|
has matured into a polished, feature-rich, free-of-charge, open source
operating system that meets the desktop or server needs of the beginner
to the advanced user alike.

|trueos| is essentially a customized installation of FreeBSD, not a
forked derivative. Since the underlying FreeBSD system has been kept
intact, you have a fully functional FreeBSD system under the hood.
|trueos| provides an easy-to-use installer which can be used to install
a desktop or a server version of FreeBSD. Other differences from FreeBSD
include: 

* |trueos| pre-configures the BSD-licensed, |lumina| desktop
  environment during a desktop installation. Additional desktop
  environments can be installed and will appear in the login menu,
  allowing the user to select which environment to log into.

* The |trueos| installer supports configuring ZFS and encryption during
  installation.

* |trueos| provides both a graphical and command line software management
  system.

* |trueos| provides many graphical utilities for configuring and managing
  the system. These utilities have both a command line equivalent and
  a REST and WebSocket API so that they can also be used to manage
  multiple systems.

* |trueos| comes pre-configured with a number of automatic scripts to
  perform tasks such as connecting digital cameras or USB memory sticks.

* The |trueos| boot menu supports boot environments, or snapshots of the
  operating system, and the |trueos| Update Manager automatically adds a
  new boot environment to the boot menu before updating the operating
  system or software. This means that if an update fails, the system can
  reboot into the previous version of the operating system, before the
  update occurred.

While it began as an independent project, since October 2006 |trueos| is
financially backed and supported by the enterprise-class hardware
solutions provider `iXsystems <https://www.ixsystems.com/>`_.

.. index:: introduction, typographic
.. _Typographic Conventions:

Typographic Conventions
=======================

The |trueos| User Guide uses several typographic conventions, seen here
in :numref:`Table %s <typconv>`:

.. _typconv:

.. table:: : Text Formatting Examples

   +-------------------------+------------------------------------------------+
   | Item                    | Visual Example                                 |
   +=========================+================================================+
   | Graphical elements:     | Click the :guilabel:`Import CA` button.        |
   | buttons, icons, fields, |                                                |
   | columns and boxes       |                                                |
   +-------------------------+------------------------------------------------+
   | Menu selections         | Click :menuselection:`System --> Information`. |
   +-------------------------+------------------------------------------------+
   | CLI Command name        | Use :command:`scp`.                            |
   +-------------------------+------------------------------------------------+
   | A command line example  | :samp:`[tmoore@example] ls /etc`               |
   +-------------------------+------------------------------------------------+
   | Files, volume and       | Locate the :file:`/etc/rc.conf` file.          |
   | dataset names, and      |                                                |
   | directories             |                                                |
   +-------------------------+------------------------------------------------+
   | Keyboard keys           | Press the :kbd:`Enter` key.                    |
   +-------------------------+------------------------------------------------+
   | Important points        | **This is important.**                         |
   +-------------------------+------------------------------------------------+
   | Values entered into     | Enter *127.0.0.1* in the address field.        |
   | fields, or device names |                                                |
   +-------------------------+------------------------------------------------+

.. index:: introduction, features
.. _Goals and Features:

Goals and Features
==================

|trueos| provides these features:

* **Easy installation:** To install either a graphical desktop or
  command-line server, simply insert the installation media, reboot the
  system to start the installer, and answer a few questions in the
  installation menus.

* **Automatically configured hardware:** Video, sound, network, and
  other devices are configured automatically during installation.

* **Intuitive desktop interface:** |trueos| installs the |lumina|
  desktop, but additional desktop environments can be installed to
  support day-to-day computing needs.

* **Easy software management:** With `AppCafe <https://sysadm.us/handbook/client/sysadmclient.html#appcafe>`_,
  installing, upgrading, and uninstalling software is safe and easy.

* **Lots of software available:** |appcafe| can be used to install
  software ported to FreeBSD (currently over 26,100 applications).

* **Easy to update:** |trueos| (with |sysadm|) provides a built-in
  `Update Manager <https://sysadm.us/handbook/client/sysadmclient.html#update-manager>`_
  which provides notifications of available updates. This utility makes
  it easy to apply operating system security fixes, bug fixes, and
  system enhancements, as well as upgrade to newer versions of the
  operating system or installed software.

* **Virus-free:** |trueos| is unaffected by viruses, spyware, or other
  malware.

* **No defragmentation:** |trueos| hard drives do not need to be
  defragmented and are formatted with OpenZFS, a self-healing filesystem.

* **Laptop support:** Provides power saving, swap space encryption, and
  automatic switching between wired and wifi network connections.

* **Secure environment:** |trueos| provides a pre-configured firewall
  and a built-in host-based Intrusion Detection System.

* **Easy system administration:** |trueos| provides many graphical tools
  for performing system administration tasks.

* **Localization:** |trueos| supports a variety of native languages and
  locales.

* **Vibrant community:** |trueos| has a friendly and helpful community.

.. index:: introduction, legal
.. _Legal:

Legal
=====

This section covers the required legal elements to the handbook,
including the Copyright notice, Trademarks used in the document, and the
|trueos| ethical advertising policy.

.. index:: introduction, legal, copyright
.. _Copyright:

Copyright & Trademarks
----------------------

Copyright © 2005-2016 iXsystems

The |trueos| User Guide is freely available for sharing and
redistribution under the terms of the
`Creative Commons Attribution License <https://creativecommons.org/licenses/by/3.0/>`_.
This means you have permission to copy, distribute, translate, and
adapt the work, as long as you attribute the |trueos| Project as the
original source of the Handbook.

|trueos| and the |trueos| logo are registered trademarks of
`iXsystems <https://www.ixsystems.com/>`_. To use the |trueos| logo in
your own works, please ask for permission first from
marketing@ixsystems.com.

|lumina| and the |lumina| logo are registered trademarks of
`iXsystems <https://www.ixsystems.com/>`_. To use the |lumina| logo in
your own works, please ask for permission first from
marketing@ixsystems.com.

|sysadm| is a trademark of `iXsystems <https://www.ixsystems.com/>`_.

|trpi|, |pise|, and |picl| are trademarks of
`iXsystems <https://www.ixsystems.com/>`_.

AMD is a trademark of Advanced Micro Devices, Inc.

Apache is a trademark of The Apache Software Foundation.

|appcafe| is a registered trademark of
`iXsystems <https://www.ixsystems.com/>`_.

Asus® and Eee PC® are registered trademarks of ASUSTeK® Computer Inc.

Facebook® is a registered trademark of Facebook Inc.

Flash® is a registered trademark of Adobe Systems Incorporated in the
United States and/or other countries.

FreeBSD® is a registered trademark of the
`FreeBSD Foundation <https://www.freebsdfoundation.org/>`_.

|freenas| is a registered trademark of
`iXsystems <https://www.ixsystems.com/>`_.

Intel, the Intel logo, Pentium Inside, and Pentium are trademarks of
Intel Corporation in the U.S. and/or other countries.

Java™ is a trademark of Oracle America and/or its affiliates in the
United States and other countries.

LinkedIn® is a registered trademark of LinkedIn Corporation.

Linux® is a registered trademark of Linus Torvalds.

Mac and Mac OS are trademarks of Apple Inc., registered in the U.S. and
other countries.

NVIDIA® is a trademark and/or registered trademark of NVIDIA Corporation
in the U.S. and other countries.

ThinkPad® is a registered trademark of Lenovo.

Twitter is a trademark of Twitter, Inc. in the United States and other
countries.

UNIX® is a registered trademark of The Open Group.

VirtualBox® is a registered trademark of Oracle.

VMWare® is a registered trademark of VMWare, Inc.

Windows® is a registered trademark of Microsoft Corporation in the
United States and other countries.

.. index:: introduction, legal, advertising
.. _Ad policy:

Ethical Advertising Policy
--------------------------

For many years, users have wanted to give back to the |trueos| project.
Generally, we encouraged users to donate or actively contribute to the
FreeBSD project to ensure FreeBSD continues to be successful in the
future. Because |trueos| is open source software, we have included a
minimal number of ads as a simple method for users to give back to the
project, if they wish. 

The primary consideration for these ads is to avoid detracting from the
user experience as much as possible. To this end, any ads in the
Handbook will be limited to the navigation sidebar, and only in a
predefined space underneath all other navigation options. We are
resolved to protect user privacy and security, and do not collect user
information, with the exception of click throughs. Furthermore, we do
not collect any data for targeted ads, and are committed to only show
high quality ads pertaining to our user base.  

**Cookie Policy**

Clicking on a Newegg ad directs users through an affiliate link that
gives the |trueos| project a modest commission based on any items
purchased within 24 hours. This is a simple time tracking cookie used to
ensure the |trueos| project is afforded its commission. To ask questions
about our Ethical Advertising policy, please contact joshms@trueos.org
for more information.

.. index:: introduction, comparing
.. _Comparing TrueOS:

Comparing |trueos|
==================

As |trueos| grows and evolves, many users appreciate comparisons with
other operating systems. These comparisons are intended to help new
users deciding to install and try |trueos|, with accuracy being
the chief concern.

.. index:: introduction, comparing, FreeBSD/PC-BSD
.. _FreeBSD and PCBSD:

FreeBSD and PC-BSD
------------------

The following features or enhancements were introduced for |trueos| and
now separate |trueos| from |pcbsd|:

.. note:: |pcbsd| and FreeBSD are placed together as both are very
   similar "under the hood". Differences for either OS to |trueos| are
   listed here.

* Based on FreeBSD-CURRENT.

* The GRUB bootloader has been replaced by the FreeBSD bootloader which
  now provides both GELI and boot environment support. The
  :guilabel:`Use GRUB bootloader` checkbox has been added to the
  :guilabel:`Customize Disk Selection` screens for users of dual-boot
  systems who prefer to use the GRUB boot loader.

* **Quick boot times with OpenRC:** |trueos| is using
  `OpenRC <https://github.com/OpenRC/openrc>`_ as part of the init
  process to start services in parallel. This results in dramatically
  improved system boot times for |trueos|. OpenRC is also used to
  improve general service management, in addition to adding the
  functionality to automatically run when new elements are introduced to
  the system, such as plugging in an ethernet cable. Use of OpenRC
  introduces a new level of differentiation from FreeBSD as |trueos| now
  uses some different system services. These differences are listed in
  :numref:`Table %s <sysserv>`
  
  .. _sysserv:
  
  .. table:: : Different system services between |trueos| and FreeBSD

     +------------------+--------------+-----------------+
     | |trueos| Service | Started From | FreeBSD Service | 
     +==================+==============+=================+
     | openntpd         | Ports        | ntpd            |
     +------------------+--------------+-----------------+
     | network          | Base         | netif           | 
     +------------------+--------------+-----------------+
     | wpa_supplicant   | Ports; Start | wpa_supplicant  |
     |                  | with network | (from Base)     |
     +------------------+--------------+-----------------+
     | dhcpcd           | Ports        | dhclient        |
     +------------------+--------------+-----------------+
     
  .. note:: :ref:`sysserv` will be updated as development continues on
     the |trueos| implementation of OpenRC. For a complete list of all
     available services through OpenRC, see :ref:`rcuprnlvl`.

* A |trueos| installation installs the |lumina| Desktop. Additional
  window managers can be installed using |appcafe|.

* The `SysAdm™ Client <https://sysadm.us/handbook/client/>`_
  and `Server <https://sysadm.us/handbook/server/>`_ has replaced
  Control Panel. Most of the utilities from the Control Panel have been
  rewritten to use the |sysadm| middleware. Under the hood, |sysadm|
  provides REST and WebSocket APIs for securely managing local and
  remote FreeBSD and |trueos| systems.

* Many utilities have been converted to the |sysadm| API and are
  available through `SysAdm <https://sysadm.us/handbook/client/>`_:

  * AppCafe
  * Update Manager
  * Boot Environment Manager
  * Life Preserver
  * Firewall Manager
  * User Manager
  * Network Manager
  * Mount Tray
  
* The functionality provided by the *About* utility has been
  incorporated into
  `Lumina Information <https://lumina-desktop.org/handbook/luminautl.html#lumina-information>`_.
  
* The functionality provided by
  `Service Manager <https://sysadm.us/handbook/client/sysadmclient.html#service-manager>`_
  (:command:`pc-servicemanager`) has been integrated into |sysadm|.

* The Active Directory & LDAP utility (:command:`pc-adsldap`) has been
  deprecated.

* Login Manager (:command:`pc-dmconf`) has been replaced by
  :command:`pcdm-config`).

* System Manager (:command:`pc-sysmanager`) has been deprecated.

* :command:`freebsd-update` has been retired in favor of using
  :command:`pkg` for system updates.

* The binary for :ref:`Disk Manager` (:command:`pc-zmanager`) has been
  renamed to :command:`pc-diskmanager` and the graphical version has
  been moved to the :guilabel:`Browse Applications` menu.

* The option to use the SCFB display driver has been added to the
  installer. This driver is suitable for newer UEFI laptops as it
  automatically detects native resolution and is a good solution for
  newer Intel drivers that have not been ported yet to FreeBSD. Before
  selecting this driver, check the BIOS and ensure the CSM module is
  disabled. This driver does not support a dual-head configuration, such
  as an external port for presentations, or suspend and resume.

* :guilabel:`Customize` has been removed from the
  :ref:`System Selection` screen in order to reduce the size of the
  installation media. Additional software can be installed
  post-installation using |appcafe|.

* The :guilabel:`Boot to console (Disable X)` option has been added to
  the graphical boot menu.

* These new utilites are available in the *SysAdm Client*
  `Managing Remote Connections <https://sysadm.us/handbook/client/sysadmclient.html#managing-remote-connections>`_
  and
  `Task Manager <https://sysadm.us/handbook/client/sysadmclient.html#task-manager>`_.

* The graphical and command line versions of PBI Manager and Warden have
  been removed.

* :command:`pc-thinclient` has been removed as it is deprecated.

.. index:: introduction, comparing, Linux
.. _Linux and TrueOS:

Linux and |trueos|
------------------

|trueos| is based on FreeBSD, meaning it is not a Linux distribution.
If you have used Linux before, you will find some features you are used
to have different names on a BSD system and some commands are different.
This section covers some of these differences.

BSD and Linux use different filesystems during installation. Many Linux
distros use EXT2, EXT3, EXT4, or ReiserFS, while |trueos| uses OpenZFS.
This means if you wish to dual-boot with Linux or access data on an
external drive formatted with another filesystem, you will want to
research if the data will be accessible to both operating systems.

:numref:`Table %s <filesys support>` summarizes the various filesystems
commonly used by desktop systems. |trueos| will automatically mount
several filesystems: *FAT16*, *FAT32*, *EXT2*, *EXT3*
(without journaling), *EXT4* (read-only), *NTFS5*, *NTFS6*, and *XFS*.
See the section on :ref:`Files and File Sharing` for a comparison of
some graphical file manager utilities.

.. _filesys support:

.. table:: : Filesystem Support on |trueos|

   +------------+-----------+-------------------------+--------------------------------------------------------+
   | Filesystem | Native to | Non-native support type | Usage notes                                            |
   +============+===========+=========================+========================================================+
   | Btrfs      | Linux     | none                    |                                                        |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | exFAT      | Windows   | none                    | requires a license from Microsoft                      |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | EXT2       | Linux     | r/w support loaded      |                                                        |
   |            |           | by default              |                                                        |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | EXT3       | Linux     | r/w support loaded      | since EXT3 journaling is not supported, you will not   |
   |            |           | by default              | be able to mount a filesystem requiring a journal      |
   |            |           |                         | replay unless you :command:`fsck` it using an          |
   |            |           |                         | external utility such as                               |
   |            |           |                         | `e2fsprogs <http://e2fsprogs.sourceforge.net>`_        |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | EXT4       | Linux     | r/o support loaded      | EXT3 journaling, extended attributes, and inodes       |
   |            |           | by default              | greater than 128 bytes are not supported; EXT3         |
   |            |           |                         | filesystems converted to EXT4 may have better          |
   |            |           |                         | performance                                            |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | FAT16      | Windows   | r/w support loaded      |                                                        |
   |            |           | by default              |                                                        |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | FAT32      | Windows   | r/w support loaded      |                                                        |
   |            |           | by default              |                                                        |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | HFS+       | Mac OS X  | none                    | older Mac versions might work with                     |
   |            |           |                         | `hfsexplorer <http://www.catacombae.org/hfsexplorer>`_ |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | JFS        | Linux     | none                    |                                                        |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | NTFS5      | Windows   | full r/w support loaded |                                                        |
   |            |           | by default              |                                                        |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | NTFS6      | Windows   | r/w support loaded      |                                                        |
   |            |           | by default              |                                                        |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | ReiserFS   | Linux     | r/o support is loaded   |                                                        |
   |            |           | by default              |                                                        |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | UFS2       | FreeBSD   | check if a Linux distro | changed to r/o support in Mac Lion                     |
   |            |           | provides ufsutils;      |                                                        |
   |            |           | r/w support on Mac;     |                                                        |
   |            |           | UFS Explorer can be     |                                                        |
   |            |           | used on Windows         |                                                        |
   +------------+-----------+-------------------------+--------------------------------------------------------+
   | ZFS        | |trueos|, |                         |                                                        |
   |            | FreeBSD   |                         |                                                        |
   +------------+-----------+-------------------------+--------------------------------------------------------+

Linux and BSD use different naming conventions for devices. For example:

* In Linux, Ethernet interfaces begin with :file:`eth`. With BSD,
  interface names indicate the name of the driver. For example, an
  Ethernet interface may be listed as :file:`re0`, indicating it uses
  the Realtek :file:`re` driver. The advantage of this convention is
  you can read the **man 4** page for the driver (e.g. type
  :command:`man 4 re`) to see which models and features are provided by
  the driver.

* BSD disk names differ from Linux. IDE drives begin with :file:`ad` and
  SCSI and USB drives begin with :file:`da`.

Some of the features used by BSD have similar counterparts to Linux, but
the name of the feature is different. :numref:`Table %s <feature names>`
provides some common examples:

.. _feature names:

.. table:: : BSD and Linux Feature Names

   +------------------------------+---------------------+--------------------------------+
   | TrueOS                       | Linux               | Description                    |
   +==============================+=====================+================================+
   | IPFW                         | iptables            | Default firewall               |
   +------------------------------+---------------------+--------------------------------+
   | :file:`/etc/rc.d/` for       | :file:`rc0.d/`,     | In |trueos|, the directories   |
   | operating system and         | :file:`rc1.d/`,     | containing the startup scripts |
   | :file:`/usr/local/etc/rc.d/` | etc.                | do not link to runlevels as    |
   | for applications             |                     | there are no runlevels. System |
   |                              |                     | startup scripts are separated  |
   |                              |                     | from third-party application   |
   |                              |                     | scripts.                       |
   +------------------------------+---------------------+--------------------------------+
   | :file:`/etc/ttys` and        | :command:`telinit`, | Terminals configured in *ttys* |
   | :file:`/etc/rc.conf`         | :file:`init.d/`     | and *rc.conf* indicate which   |
   |                              |                     | services start at boot time.   |
   +------------------------------+---------------------+--------------------------------+

Users comfortable with the command line may find some of the common
Linux commands have different names on BSD.
:numref:`Table %s <common commands>` lists some common commands and
what they are used for.

.. _common commands:

.. table:: : Common BSD and Linux Commands

   +-----------------------------------+-----------------------------+
   | Command                           | Used                        |
   +===================================+=============================+
   | :command:`dmesg`                  | discover what hardware was  |
   |                                   | detected by the kernel      |
   +-----------------------------------+-----------------------------+
   | :command:`sysctl dev`             | display configured devices  |
   +-----------------------------------+-----------------------------+
   | :command:`pciconf -l -cv`         | show PCI devices            |
   +-----------------------------------+-----------------------------+
   | :command:`dmesg | grep usb`       | show USB devices            |
   +-----------------------------------+-----------------------------+
   | :command:`kldstat`                | list all modules loaded in  |
   |                                   | the kernel                  |
   +-----------------------------------+-----------------------------+
   | :command:`kldload <module>`       | load a kernel module for    |
   |                                   | the current session         |
   +-----------------------------------+-----------------------------+
   | :command:`pkg install <pkgname>`  | install software from the   |
   |                                   | command line                |
   +-----------------------------------+-----------------------------+
   | :command:`sysctl hw.realmem`      | display hardware memory     |
   +-----------------------------------+-----------------------------+
   | :command:`sysctl hw.model`        | display CPU model           |
   +-----------------------------------+-----------------------------+
   | :command:`sysctl hw.machine_arch` | display CPU Architecture    |
   +-----------------------------------+-----------------------------+
   | :command:`sysctl hw.ncpu`         | display number of CPUs      |
   +-----------------------------------+-----------------------------+
   | :command:`uname -vm`              | get release version         |
   |                                   | information                 |
   +-----------------------------------+-----------------------------+
   | :command:`gpart show`             | show device partition       |
   |                                   | information                 |
   +-----------------------------------+-----------------------------+
   | :command:`fuser`                  | list IDs of all processes   |
   |                                   | with one or more files open |
   +-----------------------------------+-----------------------------+

There are many articles and videos which provide additional information
about some of the differences between BSD and Linux:

* `Comparing BSD and Linux <http://www.freebsd.org/doc/en/articles/explaining-bsd/comparing-bsd-and-linux.html>`_

* `FreeBSD Quickstart Guide for Linux® Users <http://www.freebsd.org/doc/en/articles/linux-users/index.html>`_

* `BSD vs Linux <http://www.over-yonder.net/~fullermd/rants/bsd4linux/01>`_

* `Why Choose FreeBSD? <http://www.freebsd.org/advocacy/whyusefreebsd.html>`_

* `Interview: BSD for Human Beings <http://www.unixmen.com/bsd-for-human-beings-interview/>`_

* `Video: BSD 4 Linux Users <https://www.youtube.com/watch?v=xk6ouxX51NI>`_

* `Why you should use a BSD style license for your Open Source Project <http://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html>`_

* `A Sysadmin's Unixersal Translator (ROSETTA STONE) <http://bhami.com/rosetta.html>`_

.. TODO Work in comparison sections with Windows and Mac OSX:
   .. index:: introduction, comparing, Windows
   .. _Windows:

   Windows
   -------

   .. index:: introduction, comparing, Mac
   .. _Mac OS:

   Mac OS
   ------