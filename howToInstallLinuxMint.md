# Introduction
This guide is made for people who know little about computers to help them install Linux Mint in a way they can understand.

# Common Terms and Questions

## What is a Linux?

## Why Linux Mint?

## Why open source?
See section on FOSS and SaaS.

### Is it dangerous to use open source systems?
short answer no
long answer no

## What is a Package Manager?
A good article written to explain this [can be found here](https://itsfoss.com/package-manager/).
Note that Linux Mint uses the `apt` and `flatpak` package managers.

### Linux Mint uses apt and flatpak. What's the difference?
The Linux Mint GUI software manager actually explains it in simple terms pretty well.

![](./assets/packageManagersLinuxMint.png)

For most software, installing the flatpak is better than the system (`apt`) package, because it is more up to date. There are some exceptions to this, like Steam.


## What is a UEFI BIOS?

In short, it stands for [**U**nified **E**xtensible **F**irmware **I**interface](https://en.wikipedia.org/wiki/UEFI) [**B**asic **I**nput **O**utput **S**ystem](https://en.wikipedia.org/wiki/BIOS)

That probably means nothing to you though and isn't very helpful. This is the case for most people, which is completely normal. Annoyingly, some people still call it the **BIOS**, though it should really be just called the **UEFI**. For the sake of clarity, in this guide it is reffered to as the **UEFI BIOS** for ease of description.

The UEFI BIOS is the level of your computer below the Operating System and is generally built into your motherboard by your manufacturer. It takes form of a simple GUI that lets you decide things such as various core hardware functions and which drive to boot from. This will be important in booting a new Operating System.

## What is "FOSS" and "SaaS"?

### SaaS kinda sucks

### Closed source is dumb

### Why open source is ideal

### FOSS is freedom

## Can I still play my games on Linux?
yes, todo
### WINE

#### Winetricks GUI
makes it easier

### Steam Proton

## What if an application I use is not availible in Linux natively?

### FOSS Alternatives (preferable)

### WINE (if you must)

# Prerequisites
This guide assumes you have a computer running Windows and would like to move to Linux Mint.
It also assumes you can use a search engine to solve problems and don't suffer from general learned helplessness.

Here's a few things you should know.

## Step -2: Ask yourself if you have any files on your Windows machine that you would like to have after the switch. 

This is because Linux uses different file system(s) to Windows, so your OS drive (generally the largest one thats not external) will need to be formatted during the install.

**If you have files you would like to keep.**
> I reccomend backing up any files you would like to keep somewhere else during the install. Purchasing an external storage to save any files you want is a great way to do this.

**If you do not care about any of the files on the machine.**
> You can safely ignore this and move to the next preparation step.

## Step -1: Get a 32GB or larger USB stick.
Do what the step says. You will need this to create a bootable USB of Linux Mint, which you will use to easily install it. Linux Mint is a different operating system, not a Windows installer program.

# Step 0: Creating the Bootable USB 

todo
## Downloading Rufus

## Downloading the .iso file

## Flashing the .iso to the USB

# Step 1: Accessing the UEFI BIOS

## Finding your UEFI BIOS key

## Entering the UEFI BIOS

# Step 2: Configuring the UEFI BIOS

## Disabling certian unwanted settings

### Fast boot

### "Secure" boot

## Changing the boot order

## Save changes and restart

# Step 3: Boot and Install

## When you boot

### If the standard boot doesn't work

## The live image
**JUST BECAUSE YOU BOOTED DOES NOT MEAN IT'S INSTALLED**

## Installing Linux Mint

### What if my wifi is not working/showing up on Linux?

# Step 4: Post-install

## Welcome Menu

## Update Manager

## Drivers (Very Important)

### Contibuation from Step 3: What if I don't have wifi in linux but I do on windows?

#### Fuck broadcom

#### Installing proprietary Wifi drivers

## Installing applications

## Reccomendations from the author

### Ublock Origin in Firefox
