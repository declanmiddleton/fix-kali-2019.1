# fix-kali-2019.1
update 2019 package

fix broken packages in kali install 2019.1


copy to (/etc/apt/sources.list)
deb http://http.kali.org/kali kali-rolling main contrib non-free
deb-src http://http.kali.org/kali kali-rolling main contrib non-free

run in terminal
apt update && apt -y full-upgrade


Fixing Unmet Dependencies Error (broken packages)

$ sudo apt-get install -f
$ sudo dpkg-configure -a
$ sudo apt-get install -f


if you get this. the error is not fixed
0 upgraded, 0 newly installed, 0 to remove, and 0 not upgraded.

run this 
$ sudo apt-get update
$ sudo apt-get install aptitude

sudo apt-get -u dist-upgrade

sudo apt-get -o Debug::pkgProblemResolver=yes dist-upgrade


clearing the package database
$ sudo apt-get clean 
$ sudo apt-get autoclean
