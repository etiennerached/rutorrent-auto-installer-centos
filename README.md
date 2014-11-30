rutorrent-auto-installer-centos
===============================

ruTorrent Auto Installer Script for CentOS and Debian/Ubuntu

This auto installer was initially found in here:
http://sourceforge.net/projects/autodl-irssi/files/autodl-setup/download

However it's no longer updated by it's original author, and most of the SVNs were outdated which broke the installation.
So I decided to fix the urls and add it in here.

How to run and install instructions:
http://www.tech-and-dev.com/2013/04/installing-rutorrent-on-centos-and-debian.html

===============================

Note for CentOS 7:
==================
Apache and mod_scgi does not work well on CentOS 7 yet. If you are on CentOS 7 You should choose nginx while installing.
And make sure to allow the http/https ports in the firewal:
sudo firewall-cmd --permanent --zone=public --add-service=http 
sudo firewall-cmd --permanent --zone=public --add-service=https
sudo firewall-cmd --reload
