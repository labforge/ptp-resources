# PTPv2 (IEEE 1588-2008) recipes for Bottlenose

Bottlenose cameras support the Precision Time Protocol (PTP). This repository contains
recipes to implement a local PTP grandmaster running on a Linux system and pointers
hot to set up Windows subscribers.

For Bottlenose to synchronize via PTP you need to have at least one PTP grandmaster
clock in your subnet. You buy a commercial clock source or setup a Linux machine
that provides the grandmaster clock. Please install ```ptpd```, a sample configuration
can be found [here](conf/ptpd.conf).

Since Windows 10 2018, Microsoft Windows has native support to operate as
ptp slave. Please follow [these instructions](https://github.com/microsoft/W32Time) 
to setup Windows clients.
