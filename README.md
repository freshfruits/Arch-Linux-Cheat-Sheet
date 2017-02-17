# Arch-Linux-Cheat-Sheet

<h1 align="center">
	<img src="https://www.archlinux.org/static/logos/archlinux-logo-dark-90dpi.ebdee92a15b3.png" alt="arch">
</h1>

Awesome Arch Linux cheat sheet, that I will mostly update from time to time, whenever I find something, that I need to remember, but find it hard to. 

### AUR
https://wiki.archlinux.org/index.php/Arch_User_Repository
~~~
/etc/pacman.conf
[archlinuxfr]
SigLevel = Never
Server = http://repo.archlinux.fr/$arch
~~~

### Pacman
Package signing
https://wiki.archlinux.org/index.php/Pacman/Package_signing

### Commands

~~~
pacman -Syy      	  # force synchronization of repository databases
pacman -Syu		 # 

pacman -Ss xyz   	# search repository database for packages for xyz
pacman -S xyz    	 # install package xyz

pacman -Sy xyz   	# synchronize repo and install xyz
pacman -Syy xyz        # really synchronize repo and install xyz

pacman -R xyz    	 # remove package xyz but keep its dependencies installed
pacman -Rs xyz   	# remove package xyz and all its dependencies (if they are not required by any other package)
pacman -Rsc xyz        # remove package xyz, all its dependencies and packages that depend on the target package
pacman -Ql xyz   	# show all files installed by the package xyz
pacman -Qo /path     # find the package which installed the file at /pat
~~~
