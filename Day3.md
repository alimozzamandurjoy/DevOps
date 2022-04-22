'''everything is a file in linux'''

some file types:
 * regular files(-), directory file (d) , block, link(l), socket, pipe(p) , special file (c)

ln -s < orignalFilePath> < LinkFilePath> 

root user 
sudo -i 


*Grep*

```
ser@user-Lenovo-ideapad-320-14IKB:~$ sudo -i
[sudo] password for user: 
root@user-Lenovo-ideapad-320-14IKB:~# ls
snap
root@user-Lenovo-ideapad-320-14IKB:~# cd snap
root@user-Lenovo-ideapad-320-14IKB:~/snap# ls
heroku  snap-store
root@user-Lenovo-ideapad-320-14IKB:~/snap# cd ..
root@user-Lenovo-ideapad-320-14IKB:~# ls
snap
root@user-Lenovo-ideapad-320-14IKB:~# mkdir test
root@user-Lenovo-ideapad-320-14IKB:~# ls
snap  test
root@user-Lenovo-ideapad-320-14IKB:~# touch test1.cfg
root@user-Lenovo-ideapad-320-14IKB:~# ls
snap  test  test1.cfg
root@user-Lenovo-ideapad-320-14IKB:~# grep firewall test1.cfg
root@user-Lenovo-ideapad-320-14IKB:~# grep Firewall test1.cfg
root@user-Lenovo-ideapad-320-14IKB:~# vim test1.cfg
root@user-Lenovo-ideapad-320-14IKB:~# grep -i firewall *
grep: snap: Is a directory
grep: test: Is a directory
root@user-Lenovo-ideapad-320-14IKB:~# grep -i firewall test1.cfg
root@user-Lenovo-ideapad-320-14IKB:~# vim test1.cfg
root@user-Lenovo-ideapad-320-14IKB:~# grep -i firewall test1.cfg
firewall 
root@user-Lenovo-ideapad-320-14IKB:~# grep -i bla test1.cfg
fire wall is disable bla bla
root@user-Lenovo-ideapad-320-14IKB:~# grep -i firewall *
grep: snap: Is a directory
grep: test: Is a directory
test1.cfg:firewall 
root@user-Lenovo-ideapad-320-14IKB:~# grep SELINUX
^C 
root@user-Lenovo-ideapad-320-14IKB:~# grep SELINUX /etc/*
grep: /etc/acpi: Is a directory
grep: /etc/alsa: Is a directory
grep: /etc/alternatives: Is a directory
grep: /etc/apm: Is a directory
grep: /etc/apparmor: Is a directory
grep: /etc/apparmor.d: Is a directory
grep: /etc/apport: Is a directory
grep: /etc/apt: Is a directory
grep: /etc/avahi: Is a directory
grep: /etc/bash_completion.d: Is a directory
grep: /etc/binfmt.d: Is a directory
grep: /etc/bluetooth: Is a directory
grep: /etc/brltty: Is a directory
grep: /etc/ca-certificates: Is a directory
grep: /etc/calendar: Is a directory
grep: /etc/chatscripts: Is a directory
grep: /etc/console-setup: Is a directory
grep: /etc/cracklib: Is a directory
grep: /etc/cron.d: Is a directory
grep: /etc/cron.daily: Is a directory
grep: /etc/cron.hourly: Is a directory
grep: /etc/cron.monthly: Is a directory
grep: /etc/cron.weekly: Is a directory
grep: /etc/cups: Is a directory
grep: /etc/cupshelpers: Is a directory
grep: /etc/dbus-1: Is a directory
grep: /etc/dconf: Is a directory
grep: /etc/default: Is a directory
grep: /etc/depmod.d: Is a directory
grep: /etc/dhcp: Is a directory
grep: /etc/dictionaries-common: Is a directory
grep: /etc/dkms: Is a directory
grep: /etc/dpkg: Is a directory
grep: /etc/emacs: Is a directory
grep: /etc/environment.d: Is a directory
grep: /etc/firefox: Is a directory
grep: /etc/fonts: Is a directory
grep: /etc/fwupd: Is a directory
grep: /etc/gdb: Is a directory
grep: /etc/gdm3: Is a directory
grep: /etc/geoclue: Is a directory
grep: /etc/ghostscript: Is a directory
grep: /etc/glvnd: Is a directory
grep: /etc/gnome: Is a directory
grep: /etc/groff: Is a directory
grep: /etc/grub.d: Is a directory
grep: /etc/gss: Is a directory
grep: /etc/gtk-2.0: Is a directory
grep: /etc/gtk-3.0: Is a directory
grep: /etc/hp: Is a directory
grep: /etc/ifplugd: Is a directory
grep: /etc/init: Is a directory
grep: /etc/init.d: Is a directory
grep: /etc/initramfs-tools: Is a directory
grep: /etc/insserv.conf.d: Is a directory
grep: /etc/iproute2: Is a directory
grep: /etc/java-11-openjdk: Is a directory
grep: /etc/kernel: Is a directory
grep: /etc/ldap: Is a directory
grep: /etc/ld.so.conf.d: Is a directory
grep: /etc/libblockdev: Is a directory
grep: /etc/libnl-3: Is a directory
grep: /etc/libpaper.d: Is a directory
grep: /etc/libreoffice: Is a directory
grep: /etc/logcheck: Is a directory
grep: /etc/logrotate.d: Is a directory
grep: /etc/modprobe.d: Is a directory
grep: /etc/modules-load.d: Is a directory
grep: /etc/mysql: Is a directory
grep: /etc/netplan: Is a directory
grep: /etc/network: Is a directory
grep: /etc/networkd-dispatcher: Is a directory
grep: /etc/NetworkManager: Is a directory
grep: /etc/newt: Is a directory
grep: /etc/openal: Is a directory
grep: /etc/openvpn: Is a directory
grep: /etc/opt: Is a directory
grep: /etc/PackageKit: Is a directory
grep: /etc/pam.d: Is a directory
grep: /etc/pcmcia: Is a directory
grep: /etc/perl: Is a directory
grep: /etc/pki: Is a directory
grep: /etc/pm: Is a directory
grep: /etc/polkit-1: Is a directory
grep: /etc/ppp: Is a directory
grep: /etc/profile.d: Is a directory
grep: /etc/pulse: Is a directory
grep: /etc/python3: Is a directory
grep: /etc/python3.8: Is a directory
grep: /etc/rc0.d: Is a directory
grep: /etc/rc1.d: Is a directory
grep: /etc/rc2.d: Is a directory
grep: /etc/rc3.d: Is a directory
grep: /etc/rc4.d: Is a directory
grep: /etc/rc5.d: Is a directory
grep: /etc/rc6.d: Is a directory
grep: /etc/rcS.d: Is a directory
grep: /etc/rsyslog.d: Is a directory
grep: /etc/sane.d: Is a directory
grep: /etc/security: Is a directory
grep: /etc/selinux: Is a directory
grep: /etc/sensors.d: Is a directory
grep: /etc/sgml: Is a directory
grep: /etc/skel: Is a directory
grep: /etc/snmp: Is a directory
grep: /etc/speech-dispatcher: Is a directory
grep: /etc/ssh: Is a directory
grep: /etc/ssl: Is a directory
grep: /etc/sudoers.d: Is a directory
grep: /etc/sysctl.d: Is a directory
grep: /etc/systemd: Is a directory
grep: /etc/teamviewer: Is a directory
grep: /etc/terminfo: Is a directory
grep: /etc/thermald: Is a directory
grep: /etc/thunderbird: Is a directory
grep: /etc/tmpfiles.d: Is a directory
grep: /etc/ubuntu-advantage: Is a directory
grep: /etc/udev: Is a directory
grep: /etc/udisks2: Is a directory
grep: /etc/ufw: Is a directory
grep: /etc/update-manager: Is a directory
grep: /etc/update-motd.d: Is a directory
grep: /etc/update-notifier: Is a directory
grep: /etc/UPower: Is a directory
grep: /etc/usb_modeswitch.d: Is a directory
grep: /etc/vim: Is a directory
grep: /etc/vulkan: Is a directory
grep: /etc/wpa_supplicant: Is a directory
grep: /etc/X11: Is a directory
grep: /etc/xdg: Is a directory
grep: /etc/xml: Is a directory
root@user-Lenovo-ideapad-320-14IKB:~# ^C
root@user-Lenovo-ideapad-320-14IKB:~# vim /etc/selinux
root@user-Lenovo-ideapad-320-14IKB:~# grep -vi firewall test1.cfg
this wil the the file 

fire wall is disable bla bla
root@user-Lenovo-ideapad-320-14IKB:~# 
```


*less* 

*more* 

*head* : show first 10 line

*tail* : show last 10 
```
root@user-Lenovo-ideapad-320-14IKB:~# less test1.cfg
root@user-Lenovo-ideapad-320-14IKB:~# more test.cf
more: stat of test.cf failed: No such file or directory
root@user-Lenovo-ideapad-320-14IKB:~# more test.cfg
more: stat of test.cfg failed: No such file or directory
root@user-Lenovo-ideapad-320-14IKB:~# more test1.cfg
this wil the the file 

fire wall is disable bla bla
firewall 
root@user-Lenovo-ideapad-320-14IKB:~# head test1.cfg
this wil the the file 

fire wall is disable bla bla
firewall 
root@user-Lenovo-ideapad-320-14IKB:~# head-1 test1.cfg
head-1: command not found
root@user-Lenovo-ideapad-320-14IKB:~# head -1 test1.cfg
this wil the the file 
root@user-Lenovo-ideapad-320-14IKB:~# tail -1 rest1.cfg
tail: cannot open 'rest1.cfg' for reading: No such file or directory
root@user-Lenovo-ideapad-320-14IKB:~# tail -1 test1.cfg
firewall 
root@user-Lenovo-ideapad-320-14IKB:~# 
```


# Progress bar 
    - file types 
    - filters
