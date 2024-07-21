# root (/) directory folder names and contents 


## Lilith's task instructions:
Write me a report inside your terminal as a markdown file listing each directory in **YOUR** root (/) and tell me 
what each folder contains and why it's named the way it is. (3)
https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard
https://youtu.be/42iQKuQodW4?si=tQgvDKnOoG6nn2Id
https://youtu.be/P0QZnAnsQ4c?si=nZmk3pAaj3Ehu4KP
https://www.markdownguide.org/

### markdown notes:

**bold**
*italics*
~cross out~
<mark>hightlight</mark>
base<sup>sup</sup> base<sub>sub</sub>
>1
>>2
>>>
>>>>4
``` 
for all x in kobayashi:  
	print("luna loves " + x)
``` 
1. hello
1. world

+ Luna
+ likes
+ cows

| Col 1 | Col 2 | 
| :---:   |  --- |
| boop| | 

- [x] trans
- [ ] cis


[Luna's website](https://le27.github.io/L-Elliott/)

<img src="pretty_lilith.jpg" width="100"/>

# Folder list
 
## bin
bin=binary  
This folder contains executables, and it's contents can always be seen in the terminal.

Most of the common terminal commands can be found here such as ls, rm, sudo, unzip, etc  

cd does not appear here. [This](https://unix.stackexchange.com/questions/59171/why-is-cd-not-a-file-in-bin#:~:text=cd%20is%20a%20shell%20builtin,itself%2C%20not%20a%20separate%20executable.) stack exchange post seems to explain why but luna doesn't really understand it right now. Maybe lilith can explain it to her.

The "which" command can be use to find binary paths.
For example "which ls" returns "/usr/bin/ls" and interesting "which cd" returns "no cd in (/usr/local/sbin:"..."bin)"


## sbin
sbin=system binary.

This is the same as "bin" but the contents can only be used by the root user. It contains some duplicates from "bin"
(luna conjectures that this is for when some features require root and some don't).

Some examples include mount, git, rm, and rmdir.

## lib
lib=libraries  

This contains libraries required by things in other directories (specifically bin and sbin). Having them here instead of with the other files has the advantage that the same data can be called from multiple places so less duplication is needed.

Some example subdirectories include: vlc, wine, vesptop, ssh, steam.

## lib64
lib64=libraries64bit

This directory serves essentially the same purpose as "lib" but is indended specifically for systems with 64-bit processors.

## usr
usr=user

This contains its own bin, sbin, and lib directories with the same purpose as described above. These are indended to be accessed by the user more so than the other copies with the same name.  
This also makes it easier to reduce interference between manually installed
packages and those installed with a package manager.

## etc
etc=editable text config

This is where most config files are stored so they can be easily locaded and edited to customise software.
 
Although notably luna's hyperland configs are here: "~/.config/hypr"


## home
Also sometimes denoted by a ~

This contains a folder for each user. Thus luna's home directory contains only one folder called "luna". These directories contain this specific to each user. It can only be accesed by that user or someone more powerful (e.g root).

The folders "Documents", "Downloads", "Videos", and similar for each user are in these folders here.


## boot
This folder alledgedly contains the linux kernel and things needed to boot the system.  

Luna's boot folder contains   
"efi", "initramfs-linux-fallback.img", "intel-ucode.img", "grub", "initramfs-linux.img", and "vmlinuz-linux"

Luna doesn't understand what any of these are, but luna doesn't think she'll want to ever interact with this folder until she has a much higher power level.

## dev
dev=device files

This folder is for hardware and drivers.   

Some example contents are the "cpu" folder, the "core" folder, various "loop" files, and many more.

Luna doesn't understand what any of these are, but luna doesn't think she'll want to ever interact with this folder until she has a much higher power level.


## opt
opt=optional

This directory is for software addons. Luna's "opt" directory contains the folders "beeper", "google", "pokemon-colorscripts", and "zoom". The pokemon one is presumably for the pokemon art which appear in the terminal.

## var
var=variable

This is for logs and cache files. some example folders include "empty", "cache", "games", "log", "run", and many others.  

Luna doesn't understand this well, but luna doesn't think she'll want to ever interact with this folder until she has a much higher power level.


## tmp
tmp=temporary

This is for files which are intended to be removed between reboots.

Some example subdirectories include "ystemd-private-5b4458d9a779443aafd200183303d4fa-bluetooth.service-79fd0n", "snap-private-tmp", ".font-unix" and many more.

Luna doesn't understand what any of these are, but luna doesn't think she'll want to ever interact with this folder until she has a much higher power level.


## lost+found
Luna seemingly cannot access this directory. Maybe lilith can show her how.

Apparently broken stuff is put here when there is a crash etc.

## mnt
mnt=mount

This is often (not necessarily) where things are mounted.

Luna's "mnt" directory is empty.

## proc
proc=process

According to google: "The /proc directory is NOT a real file system but a virtual file system that is created dynamically by Linux to provide access to certain types of hardware information and information about the running processes. It is mapped to /proc and mounted at boot time.
psudofile system which contains info about all active processes." Luna only vaguely understands this.

Luna's "proc" directory contains folders named for integers between 1 and 31956 (with many missing but including most of the first 100). It also contains a few itger files for example "consoles", "devices", and "keys".

Luna doesn't understand what any of these are, but luna doesn't think she'll want to ever interact with this folder until she has a much higher power level.

## root
Luna cannot access this directory. 

Apparently this is the home directory for root user. Luna doesn't understand this, is it diffent from the "/" directory?

## run
This directory contains info on what has run since boot.

Luna's "run" directory contains folders named "avahi-daemon", "mount", "sudo", "user", "log", and many others.

Luna doesn't understand what any of these are, but luna doesn't think she'll want to ever interact with this folder until she has a much higher power level.


## snap
Contains files related to snap packages.  

Luna's "snap" directory contains folders named "remarkable-desktop", "snapd", "wine-platform-6-stable", "bin", and many others.


## srv
srv=server

Allegedly this is not used much but is for files served by webserver.

Luna's "srv" directory contains only the directories "ftp" and "http".

## sys
sys=system

This folder contains info on devices, drivers, and "kernel features". It seems similar to "proc".

Luna's "sys" directory contains folders named "block", "class", "devices", "fs", and many others.

Luna doesn't understand what any of these are, but luna doesn't think she'll want to ever interact with this folder until she has a much higher power level.





