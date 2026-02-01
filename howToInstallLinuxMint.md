# Introduction
This guide is made for people who know little about computers to help them install Linux Mint in a way they can understand.

If you have a specific question, feel free to create an issue with the "Question" type in the repo. I'll try to answer them. Please be coherent in your asks, I don't want any question like "my screen looks weird" with a grainy image and no description.
# Common Terms and Questions

## Why switch?
There are many reasons one may want to switch to a Linux based operating system.
### Windows is ass
For one, windows sucks. It's bloated, full of spyware that tracks your every move, has ads built into the OS, and is full of bloat. Searching a singular folder should not take 30 seconds. It dosen't on Linux.

Windows is also closed source and paid, which is bad in itself. Imagine buying a car, and then when you open up the engine, instead there is just a few plugs and a giant black cube. That's what closed source software is like.
### Care about your privacy
Windows violates your privacy constantly. With recall screenshotting you, and it tracking whenever you start an app. Debloaters can only help so much. Why use an operating system designed to exploit the user for profit rather than working with them?

## What is a Linux?
Linux is *technically* just the [kernel](https://en.wikipedia.org/wiki/Kernel_(operating_system)).  But when people say [Linux](https://en.wikipedia.org/wiki/Linux), they are generally reffering to a distribution, or ["**distro**"](https://en.wikipedia.org/wiki/Linux_distribution) of the [Linux Kernel](https://en.wikipedia.org/wiki/Linux_kernel).

### The Linux Kernel

### Distributions
A distribution, or "distro", is generally an OS built off of the Linux Kernel, often utilizing GNU and FOSS components to make a desktop operating system. Different distros may be designed for different things and use different pieces of software and have differing levels of ease of use.

There may be distros designed for other things (like [OpenWRT](https://en.wikipedia.org/wiki/OpenWrt)), but that's beyond the scope of this guide. Here we will talk about desktop and user oriented distros.

## Why Linux Mint?

Linux Mint is a very user friendly distro. You can do most basic tasks without needing to use the command line. It's also very stable, and won't just break.

### User Friendliness
It has full GUI that's capable of doing tasks without needing the terminal, which makes it more comfortable for refugees from Microsoft Windows that are not used to the command-line yet.

### Stability & Reliability
Linux Mint is a stable and reliable distro that is focused on that rather than being bleeding-edge.
It also comes with a handy *Timeshift* backup tool, so if you happen to break something, you can just roll back all the important system files that you broke.

### Less Terminal Required
Linux Mint has many GUIs for doing most tasks, minimizing the need to use the command line, if at all. This is often a bonus for new users. However, learning the command line should be something most users do in time on their own.

## Why open source?
See section on FOSS and SaaS.

### Is it dangerous to use open source systems?
No. Code is reviwed and worked on by many developers around the world, and bugs are fixed quickly.

## What is a Package Manager?
A good article written to explain this [can be found here](https://itsfoss.com/package-manager/).
Note that Linux Mint uses the `apt` and `flatpak` package managers.

### Linux Mint uses apt and flatpak. What's the difference?
The Linux Mint GUI software manager actually explains it in simple terms pretty well.

![](./assets/packageManagersLinuxMint.png)

For most software, installing the flatpak is better than the system (`apt`) package, because it is more up to date. There are some exceptions to this, like Steam.

## What is a UEFI BIOS?

In short, it stands for [**U**nified **E**xtensible **F**irmware **I**nterface](https://en.wikipedia.org/wiki/UEFI) [**B**asic **I**nput **O**utput **S**ystem](https://en.wikipedia.org/wiki/BIOS)

That probably means nothing to you though and isn't very helpful. This is the case for most people, which is completely normal. Annoyingly, some people still call it the **BIOS**, though it should really be just called the **UEFI**. For the sake of clarity, in this guide it is reffered to as the **UEFI BIOS** for ease of description.

The UEFI BIOS is the level of your computer below the Operating System and is generally built into your motherboard by your manufacturer. It takes form of a simple GUI that lets you decide things such as various core hardware functions and which drive to boot from. This will be important in booting a new Operating System.

## What is "FOSS" and "SaaS"?

### SaaS kinda sucks

SaaS stands for [Software as a Service](https://en.wikipedia.org/wiki/Software_as_a_service). Although sounding mundane, it is often a predatory system wherein you don't actually own anything, and don't know how the software you use works or what data it collects because it is closed source. Generally not ideal.

> SaaS separates "the possession and ownership of software from its use."

Examples of SaaS companies could be Adobe, Todo, and Todo.

### Closed source is dumb
Imagine paying for a software and not even knowing what it does or how to fix it. It's an enigma. You have no way to know what it does without your permission, and the company randomly breaks stuff. Sound familiar? Microsoft Windows is a closed source SaaS system.

SaaS companies (like Microsoft) also have a record of knowing about significant security vulnerabilities, but not spending time to patch them until a massive hack happens because it saves them money in the short term.

### Why open source is ideal
Open source means that the source code for a piece of software is visible to the public. This means people can independently verify that it is safe and does not spy on you, plus people can contribute to a lot of open source projects to improve them.

If a bug or security issue is found, the devs are obligated to fix it via common sense. If they don't, someone will just make a fork where that bug is fixed and everyone will start using that instead.

### FOSS is freedom
Controlling your software is important. Without that control, you only have the freedom that the company making it says is allowed. With FOSS, you can do whatever you want.

## Can I still play my games on Linux?
Yes.
For some games, they have a release that is Native to Linux, and so will just run normally.
In the case a game does not have a Native to Linux release, most users will utilize WINE and Steam Proton to play those games.
### WINE

WINE is a compataiblity layer that translates Microsoft Windows function calls into POSIX-compliant function calls, with negligible performance overhead. It's not an emulator.

#### Wait but how does it work?
**The easiest way I can explain how WINE works is something like this:**

*Note: These are not real functions and this is heavily simplified. I am just making an example.*


Let's say Microsoft Windows has a function `OpenFile(name, path)`. It opens a file, and takes two arguments, the `name` of the file and the `path` to said file on the filesystem.

Linux has a similar function `fOpen(location)`. This function also opens a file, but it has a different name and only takes one argument, `location`, which just points directly to where the file is on the filesystem.

WINE translates between the two. So when a game built for Microsoft Windows is running via WINE, it would call `FileOpen(test.txt, C:\PATH\TO\FILE\)`. WINE will see this and make Linux do `fOpen(/path/to/file/test.txt)`, and return the result in a way the Microsoft Windows program can understand. 

This is a very simplified and unrealistic explanation, but it gets the point across.


#### Winetricks GUI
There is a GUI implementation of some WINE usage with the `winetricks` package. It also allows for some advanced configuration.

### Steam Proton
Steam Proton is a fork of WINE made by Valve. It's the same technology that lets Windows native games run on the Steam deck, and Steam on Linux comes with it by default, which you can use to run your entire Steam Library. 

If you want to see if a game will run on WINE/Proton, head over to `protondb` and check.

## What if an application I use is not availible in Linux natively?

### FOSS Alternatives (preferable)
The first and ideal option here is to find a FOSS software that does a similar thing to what you need while being native to Linux.

### WINE (if you must)
If a software does not have native Linux support, with some basic tinkering ypu can usually get it installed and running via WINE or [Winboat](https://www.winboat.app/) (which is like a mini virtual machine that can run any windows program seamlessly, but is not very good for games so it was not mentioned here).

## Can I use INSERT_SOFTWARE_NAME_HERE on Linux?

Use your preffered search engine. If there is a Ubuntu or Linux Mint `.deb` package availible, or a flatpak, then you are good.

### WINE and Compatability Layers (See games section)
You can use compatability layers to run non-native software.

### Using software that is hostile to your OS choice and why thats really not making the situation any better

### "But I need MS office for work/school!!!11!!"

## I need a software that does INSERT_THING_HERE on Linux! (FOSS Software Alternatives List)

### 2D Graphics

### 3D Graphics

### CAD

### Audio

### Video

### Documents

### Coding

### Text Editors

### Cloud Systems



# Prerequisites
This guide assumes you have a computer running Windows and would like to move to Linux Mint.
It also assumes you can use a search engine to solve problems and don't suffer from general learned helplessness or critical thinking deficency.

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
