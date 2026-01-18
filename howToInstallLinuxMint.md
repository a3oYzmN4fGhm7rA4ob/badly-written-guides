# Introduction
This guide is made for people who know little about computers to help them install Linux Mint in a way they can understand.

# Common Terms and Questions

## What is a Linux?
Linux is *technically* just the [kernel](https://en.wikipedia.org/wiki/Kernel_(operating_system)).  But when people say [Linux](https://en.wikipedia.org/wiki/Linux), they are generally reffering to a distribution, or "[**distro**"](https://en.wikipedia.org/wiki/Linux_distribution) of the [Linux Kernel](https://en.wikipedia.org/wiki/Linux_kernel).

### The Linux Kernel

### Distributions
A distribution, or "distro", is generally an OS built off of the Linux Kernel, often utilizing GNU and FOSS components to make a desktop operating system. Different distros may be designed for different things and use different pieces of softwarev and have differing levels of ease of use.

There may be distros designed for other things (like [OpenWRT](https://en.wikipedia.org/wiki/OpenWrt)), but that's beyond the scope of this guide. Here we will talk about desktop and user oriented distros.

## Why Linux Mint?

Linux Mint is a very user friendly distro. You can do most basic tasks without needing to use the command line. It's also very stable, and won't just break.

### User Friendliness
It has full GUI that's capable of doing tasks without needing the terminal, which makes it more comfortable for refugees from Microsoft Windows that are not used to the command-line yet.

### Stability & Reliability

### Less Terminal Required

## Why command line?

### Can't everything just be a GUI

### Learning the command line is very helpful

### Don't be afraid of it

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

SaaS stands for [Software as a Service](https://en.wikipedia.org/wiki/Software_as_a_service). Although sounding mundane, it is often a predatory system wherein you don't actually own anything, and don't know how the software you use works or what data it collects because it is closed source. Generally not ideal.

> SaaS separates "the possession and ownership of software from its use."

Examples of SaaS companies could be Adobe, Todo, and Todo.

### Closed source is dumb
Imagine paying for a software and not even knowing what it does or how to fix it. It's an enigma. You have no way to know what it does without your permission, and the company randomly breaks stuff. Sound familiar? Microsoft Windows is a closed source SaaS system.

### Why open source is ideal
Open source means that the source code for a piece of software is visible to the public. This means people can independently verify that it is safe and does not spy on you, plus people can contribute to a lot of open source projects to improve them.

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
