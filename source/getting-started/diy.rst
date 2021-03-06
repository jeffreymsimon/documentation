.. _diy:

*********
DIY Guide
*********

.. figure:: /_static/images/diy/pi.png
  :width: 40%
  :alt: Raspberry Pi

  Raspberry Pi Board

By popular demand, we are pleased to present this "Do it Yourself" (DIY) guide for the Start9 Embassy personal server!

Motivation
==========

There are four reasons you might prefer to build your own Embassy instead of purchasing one from us.

#. You already have a Raspberry Pi and would like to re-purpose it.

#. You want to save on shipping costs.

#. You prefer not to divulge your physical shipping address.

#. You just like building things.

Hardware
========

Components
----------
#. `Raspberry Pi 4B (4GB) <https://raspberrypi.org/products/raspberry-pi-4-model-b/?variant=raspberry-pi-4-model-b-4gb>`_
#. `Power supply for Raspberry Pi 4B <https://raspberrypi.org/products/type-c-power-supply/>`_
#. Case for Raspberry Pi 4B (`passive cooling recommended <https://www.amazon.com/Geekworm-Raspberry-Aluminum-Passive-Heatsink/dp/B07Z6FYHCH/>`_ `*`)
#. `High endurance microSD <https://amazon.com/SanDisk-Endurance-microSDXC-Adapter-Monitoring/dp/B07NY23WBG/>`_ (recommended 128GB or more)
#. `GPIO mini speaker/buzzer <https://amazon.com/dp/B07F8NXHGP/>`_
#. Ethernet cable
#. MicroSD → USB adapter (if no microSD port on your computer)

`*` If you use a fan, **DO NOT** use the official Raspberry Pi fan, as it requires the same GPIO pins as the audio speaker. Instead, we recommend `this fan <https://www.amazon.com/Raspberry-iUniker-30x30x7mm-Brushless-RetroFlag/dp/B076H3TKBP/>`_.

Assembly Instructions
---------------------

1. Insert mini speaker/buzzer into GPIO pins 6/8/10/12 with the word "speaker" facing out, `away from the board`.

.. figure:: /_static/images/diy/pins.png
  :width: 60%
  :alt: Speaker board spec

That's it. Place the Raspberry Pi 4 board (with speaker attached), into its case.

Getting EmbassyOS
=================

Purchasing
----------

You can purchase EmbassyOS `here <https://images.start9labs.com/order>`_. This is by far the easiest path to get up and running.

Depending on your Internet speed, the download should take between 5 and 30 minutes.

Building from Source
--------------------

If you have the proper tooling and are comfortable using the command line, you can build EmbassyOS from `source <https://github.com/Start9Labs/embassy-os>`_, which is made available under the `Start9 Personal Use License <https://start9labs.com/license>`_.

Installing EmbassyOS
====================

Whether you purchase EmbassyOS from us or build it yourself, you need to flash it onto a microSD card.

1. Download `balenaEtcher <https://www.balena.io/etcher/>`_ onto your Mac, Windows, or Linux computer.
2. Insert the microSD card into your computer, either directly or using an adapter.
3. Open balenaEtcher.
4. Click `Select Image`, then find and select your copy of EmbassyOS.
5. Click `Select Target`, then find and select your micro SD card.
6. Click `Flash!` You may be asked to (1) approve the unusually large disk target or (2) enter your password. Both are normal.

.. figure:: /_static/images/diy/balena.png
  :width: 60%
  :alt: Balena Etcher Dashboard

7. Once the image is flashed and verified, you may remove the micro SD and insert it into your Embassy.
8. The Embassy is now ready for use, and you may following the normal :ref:`setup <initial-setup>` instructions. ``*``

``*`` The first time you power it on, your Embassy will make more noises than future attempts, and it may take several minutes to finally complete.