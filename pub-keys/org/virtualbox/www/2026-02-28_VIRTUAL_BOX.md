# Virtual Box 2026-02-28

VirtualBox can be slightly challenging to install but it's worth it. You may need to mess around with your BIOS settings, etc. but eventually you should get it running. Good luck! :)

- [Virtual Box Downloads](https://www.virtualbox.org/wiki/Downloads)

Verify the integrity with sha512;

```gitbash
cd ~
git clone https://github.com/adligo/pub-keys.adligo.org.git

cd ~/Downloads
sha512sum VirtualBox-7.2.6a-172322-Win.exe > VirtualBox-7.2.6a-172322-Win.exe.sha512
cat  VirtualBox-7.2.6a-172322-Win.exe.sha512
diff VirtualBox-7.2.6a-172322-Win.exe.sha512 ~/pub-keys.adligo.org/pub-keys/org/virtualbox/www/wiki/Downloads/VirtualBox-7.2.6a-172322-Win.exe.sha512 

```

Note Docker doesn't seem to version number the installer, but I have Docker Desktop Installers of various sizes on my machine so they are clearly updating it from time to time.  You should contribute to this project and commit the sha512 checksums that you are seeing!