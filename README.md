<h3 align="center">Space cloak is an experimental project aims to provide minimal supplement for hardening linux with a few shell scripts</h3>

<br>

Space cloak is produced independently of, with no guarantee from, Arch Linux or The Tor project. Hidden cloak is created by a few individuals in their spare time. Hidden cloak was created by self-taught hobbyists in their spare time, without the backing of any particular formal certification or training. Although Hidden cloak attempts to be usable as possible, there are many ways in which it fails.

<br>

**It is recommended to install this in a Virtualization software like KVM or virtualbox.**

## How to use

First, boot with the [lastest Arch Linux ISO](https://www.archlinux.org/download/) in [Virtualbox](https://wiki.archlinux.org/index.php/VirtualBox) or [KVM](https://wiki.archlinux.org/index.php/KVM)

For some reasons, if you are planning to install this on bare metal then make sure you have Internet connection on the Arch iso. If you have a wireless connection the [`iwctl`](https://wiki.archlinux.org/index.php/Iwd#iwctl) command might be useful to you. You can also read the [Network configuration](https://wiki.archlinux.org/index.php/Network_configuration) from the Arch Linux guide for more detailed instructions.

Install [Git](https://wiki.archlinux.org/index.php/Git) then clone this repo.

<br>

To, launch the script:

```bash

chmod +x base.sh && ./base.sh

```



#### Why you should use space cloak?

- user-centrality. (because, arch linux)


#### There are already some great hardened distributions like [whonix](https://www.whonix.org/) focussing on providing privacy, security and anonymity.

- Yes, space cloak is bascially some shell scripts that runs top of arch linux, you can always start tikering with it. It is up to the user and their threat model whether to use it or not. There are many ways in which it fundamentally fails.


#### What is the purpose of space cloak ?

- In the beginning, space cloak was just an install script for arch linux with encryption by default (everything automated) and later we decided to tinker with it and we took a step further to improve by implementing more security and privacy oriented features.


#### What are the disadvantages ?

- Space cloak lacks major privacy and security enhancement like [Keystroke Deanonymization](https://github.com/vmonaco/kloak), [Boot Clock Randomization](https://github.com/Whonix/bootclockrandomization), System wide tor routing, [Hardened memory allocator](https://github.com/Whonix/hardened_malloc),  A [hardened kernel](https://source.android.com/devices/architecture/kernel/hardening) and much more, But still you can implement it, if you have the knowledge or literally start learning by doing this process. In the long run this will definitely benefit you.


#### Why Arch linux ?

- It is lightweight, minimal, rolling release and just a personal preference nothing else, it is not used for security.


#### What about other distribution ?

- These shell scripts are not written with arch linux in mind. (except the base install script which is heavily tailored towards arch linux, but still you can modify them with ease) You can always port these shell scripts to your distribution of choice, these scripts are written with great readability and less complexity. (most of them are one liners and small functions) So being minimal and less prone to bloat will reduce headaches while maintaining the whole thing. For example, if you are planing to use this in a non systemd distro like [artix linux](https://artixlinux.org/), all you have to do is replace some random line here and there.

#### I want the script that give X feature, but not interested in Y and Z scripts

- These scripts are modular, not heavily integrated to each other in any manner. Tinker with them and use it as you wish


#### Cloak script's highlights

- Base installation with encryption (fully automated)

- Uses wayland instead of Xorg (sway window manager in our case)

- Strong firewall rules 

- Strong apparmor profiles (ongoing effort)

- System wide hardening (ongoing effort)




#### Maintained by [yperta](https://github.com/yperta), [S-thirtyfive](https://github.com/S-ThirtyFive) and [Mr-mittens](https://github.com/Mr-Mittens)


Thanks to 

- [Arch Linux security](https://wiki.archlinux.org/index.php/Security)

- [Whonix wiki](https://www.whonix.org/wiki/Documentation)


***Your pull requests are always welcome***






























