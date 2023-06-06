```
$ sudo apt-get install net-tools    [On Debian/Ubuntu & Mint] 
$ sudo dnf install net-tools        [On CentOS/RHEL/Fedora and Rocky Linux/AlmaLinux]
$ pacman -S netstat-nat             [On Arch Linux]
$ emerge sys-apps/net-tools         [On Gentoo]
$ sudo dnf install net-tools        [On Fedora]
$ sudo zypper install net-tools     [On openSUSE]
```

```
$ netstat -ltnp | grep -w ':80' 
```
```
l – tells netstat to only show listening sockets.
t – tells it to display tcp connections.
n – instructs it to show numerical addresses.
p – enables showing of the process ID and the process name.
grep -w – shows matching of exact string (:80).
```
---
```
$ sudo apt-get install lsof     [On Debian, Ubuntu and Mint]
$ sudo yum install lsof         [On RHEL/CentOS/Fedora and Rocky Linux/AlmaLinux]
$ sudo emerge -a sys-apps/lsof  [On Gentoo Linux]
$ sudo pacman -S lsof           [On Arch Linux]
$ sudo zypper install lsof      [On OpenSUSE] 
```
```
$ lsof -i :80
```

---
```
$ sudo apt-get install psmisc     [On Debian, Ubuntu and Mint]
$ sudo yum install psmisc         [On RHEL/CentOS/Fedora and Rocky Linux/AlmaLinux]
$ sudo emerge -a sys-apps/psmisc  [On Gentoo Linux]
$ sudo pacman -S psmisc           [On Arch Linux]
$ sudo zypper install psmisc      [On OpenSUSE]    
```
```
$ fuser 80/tcp
```
```
$ ps -p 2053 -o comm=
$ ps -p 2381 -o comm=
```
