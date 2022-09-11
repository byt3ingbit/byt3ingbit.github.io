---
layout: default
---

## Linux Kernel Emulation with Buildroot and QEMU 

This page steps through the process in setting up an emulated environment for kernel hacking using Buildroot and QEMU.


# Dependencies  

buildroot
qemu
linux kernel source

# Getting started
Let's start clean with a new directory and environment variables.

$mkdir emulation
$cd emulation

$tar xvf buildroot-XXXX.XX.X.tar.gz


# Customizing linux kernel
Many of the configurations depend on your kernel version but there a some core configurations that we will make to the environment.
Some general tips before we dive into configurations:
setup your environment:

export ARCH=arm
export CROSS_COMPILE=arm-linux-gnueabi


# Customizing Buildroot
Buildroot does a fantastic job of building a custom kernel and filesystem. However, there are a few changes that we will make in order to setup for kernel hacking to make our lives easier.

1. Setup communication to and from your host
    a. Using ssh we need to configure a few settings





[back](./)
