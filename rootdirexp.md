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
bin=binary, contains executables, can always be seen my terminal.
e.g ls, rm, sudo, unzip 
seemingly not cd


## sbin
sbin=system binary.
same as above but contents can only be used by root user (contains some duplicates from above 
(probably for when some functions require root and some don't))
e.g mount, git, rm, rmdir

## lib
lib=libraries
is called from both bin and sbin

## lib64
lib64=libraries64bit
this is self explanatory

## usr
usr=user
contains usr targeted bin, sbin, and lib directories with same function as above.
Also contains a local directory with its own bin directory so there is no interference between manually installed
packages and those installed with a package manager

## etc
etc=editable text config
stores most config files so they can be easily edited to customise your software


## home
sometimes denoted by a tilda
folder for each user. you have only one folder called "luna". Contains stuff specific to user. can only be accesed
by that user or someone more powerful (e.g root)


## boot
contains linux kernel and things needed to boot system

## dev
dev=device files
for hardware and drivers

## opt
opt=optional
for addons

## var
var=variable
logs and cache

## tmp
tmp=temporary
removed between reboots

## lost+found
cannot access
broken stuff is put here when there is a crash etc.

## mnt
mnt=mount
where you mount stuff

## proc
proc=process
psudofile system which contains info about all active processes 

## root
cannor access
home directory for root user

## run
contains info on what has run since boot


## snap
contains files related to snap packages

## srv
srv=server
not used much
for files served by webserver

## sys
sys=system
info on devices, drivers, and "kernel features"
similar to proc


a~a~





"which" command finds binary path.
for example "which ls" returns "/usr/bin/ls"
interesting "which cd" returns "no cd in (/usr/local/sbin:"..."bin)"
