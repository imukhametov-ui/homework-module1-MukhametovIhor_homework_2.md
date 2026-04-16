ubuntu@ubuntu-VirtualBox:~$ cd /
ubuntu@ubuntu-VirtualBox:/$ ls
bin    dev   lib    libx32      mnt   root  snap      sys  var
boot   etc   lib32  lost+found  opt   run   srv       tmp
cdrom  home  lib64  media       proc  sbin  swapfile  usr
ubuntu@ubuntu-VirtualBox:/$ cd /etc
ubuntu@ubuntu-VirtualBox:/etc$ ls
acpi                           hostid               ppp
adduser.conf                   hostname             printcap
alsa                           hosts                profile
alternatives                   hosts.allow          profile.d
anacrontab                     hosts.deny           protocols
apg.conf                       hp                   pulse
apm                            ifplugd              python3
apparmor                       init                 python3.10
apparmor.d                     init.d               rc0.d
apport                         initramfs-tools      rc1.d
appstream.conf                 inputrc              rc2.d
apt                            insserv.conf.d       rc3.d
avahi                          ipp-usb              rc4.d
bash.bashrc                    iproute2             rc5.d
bash_completion                issue                rc6.d
bash_completion.d              issue.net            rcS.d
bindresvport.blacklist         kernel               resolv.conf
binfmt.d                       kernel-img.conf      rmt
bluetooth                      kerneloops.conf      rpc
brlapi.key                     ldap                 rsyslog.conf
brltty                         ld.so.cache          rsyslog.d
brltty.conf                    ld.so.conf           rygel.conf
ca-certificates                ld.so.conf.d         sane.d
ca-certificates.conf           legal                security
ca-certificates.conf.dpkg-old  libao.conf           selinux
chatscripts                    libaudit.conf        sensors3.conf
console-setup                  libblockdev          sensors.d
cracklib                       libnl-3              services
cron.d                         libpaper.d           sgml
cron.daily                     libreoffice          shadow
cron.hourly                    locale.alias         shadow-
cron.monthly                   locale.gen           shells
crontab                        localtime            skel
cron.weekly                    logcheck             snmp
cups                           login.defs           speech-dispatcher
cupshelpers                    logrotate.conf       ssh
dbus-1                         logrotate.d          ssl
dconf                          lsb-release          subgid
debconf.conf                   machine-id           subgid-
debian_version                 magic                subuid
default                        magic.mime           subuid-
deluser.conf                   mailcap              sudo.conf
depmod.d                       mailcap.order        sudoers
dhcp                           manpath.config       sudoers.d
dictionaries-common            mime.types           sudo_logsrvd.conf
dkms                           mke2fs.conf          sysctl.conf
dpkg                           ModemManager         sysctl.d
e2scrub.conf                   modprobe.d           systemd
emacs                          modules              terminfo
environment                    modules-load.d       thermald
environment.d                  mtab                 thunderbird
ethertypes                     nanorc               timezone
firefox                        netconfig            tmpfiles.d
fonts                          netplan              ubuntu-advantage
fprintd.conf                   network              ucf.conf
fstab                          networkd-dispatcher  udev
fuse.conf                      NetworkManager       udisks2
fwupd                          networks             ufw
gai.conf                       newt                 update-manager
gdb                            nftables.conf        update-motd.d
gdm3                           nsswitch.conf        update-notifier
geoclue                        openvpn              UPower
ghostscript                    opt                  usb_modeswitch.conf
glvnd                          os-release           usb_modeswitch.d
gnome                          PackageKit           vim
groff                          pam.conf             vtrgb
group                          pam.d                vulkan
group-                         papersize            wgetrc
grub.d                         passwd               wpa_supplicant
gshadow                        passwd-              X11
gshadow-                       pcmcia               xattr.conf
gss                            perl                 xdg
gtk-2.0                        pki                  xml
gtk-3.0                        pm                   zsh_command_not_found
hdparm.conf                    pnm2ppa.conf
host.conf                      polkit-1
ubuntu@ubuntu-VirtualBox:/etc$ cd /home
ubuntu@ubuntu-VirtualBox:/home$ ls
ubuntu
ubuntu@ubuntu-VirtualBox:/home$ ^C
ubuntu@ubuntu-VirtualBox:/home$ 
//завдання 2
ubuntu@ubuntu-VirtualBox:/home$ cd ~
ubuntu@ubuntu-VirtualBox:~$ mkdir lab2
ubuntu@ubuntu-VirtualBox:~$ cd lab2
ubuntu@ubuntu-VirtualBox:~/lab2$ touch file.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ cp file.txt file_copy.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ mv file_copy.txt file_renamed.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ln file.txt hard_link.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ find ~ -name "file.txt"
/home/ubuntu/lab2/file.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ls -1
file_renamed.txt
file.txt
hard_link.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ln -s file.txt soft_link.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ls -1
file_renamed.txt
file.txt
hard_link.txt
soft_link.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ^C
ubuntu@ubuntu-VirtualBox:~/lab2$ ^C
ubuntu@ubuntu-VirtualBox:~/lab2$ 
//завдання 3
ubuntu@ubuntu-VirtualBox:~/lab2$ ls -1 file.txt
file.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ chmod 444 file.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ls -1 file.txt
file.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ chmod u+w file.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ^C
ubuntu@ubuntu-VirtualBox:~/lab2$ ls -1 file.txt
file.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ umask
0022
ubuntu@ubuntu-VirtualBox:~/lab2$ umask 022
ubuntu@ubuntu-VirtualBox:~/lab2$ touch test.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ls -1 test.txt
test.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ls -1
file_renamed.txt
file.txt
hard_link.txt
soft_link.txt
test.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ls -l file.txt
-rw-r--r-- 2 ubuntu ubuntu 0 кві 16 22:22 file.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ ls -l test.txt
-rw-r--r-- 1 ubuntu ubuntu 0 кві 16 23:45 test.txt
ubuntu@ubuntu-VirtualBox:~/lab2$ sudo adduser trainee
[sudo] пароль до ubuntu: 
Вибачте, повторіть спробу.
[sudo] пароль до ubuntu: 
Вибачте, повторіть спробу.
[sudo] пароль до ubuntu: 
Додається користувач "trainee"...
Додається нова група "trainee" (1001)...
Додається новий користувач "trainee" (1001) з групою "trainee"...
Створюється домашня директорія "/home/trainee"...
Копіюються файли з "/etc/skel"..
Новий пароль: 
Повторіть новий пароль: 
passwd: пароль було успішно змінено
Зміна інформації про користувача trainee
Введіть нове значення або натисніть ENTER для типового значення
	Ім'я повністю []: ihor
	Номер кімнати []: 01
	Робочий телефон []: 038
	Домашній телефон []: 048
	Інше []: 0000
Чи є ця інформація вірною? [Т/н] t
ubuntu@ubuntu-VirtualBox:~/lab2$ sudo usermod -aG sudo trainee
ubuntu@ubuntu-VirtualBox:~/lab2$ cat /etc/passwd | grep trainee
trainee:x:1001:1001:ihor,01,038,048,0000:/home/trainee:/bin/bash
ubuntu@ubuntu-VirtualBox:~/lab2$ groups trainee
trainee : trainee sudo
ubuntu@ubuntu-VirtualBox:~/lab2$ 

