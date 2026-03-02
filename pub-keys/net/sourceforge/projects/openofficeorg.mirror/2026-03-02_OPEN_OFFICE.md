
- [https://sourceforge.net/projects/openofficeorg.mirror/](https://sourceforge.net/projects/openofficeorg.mirror/)

```
cd ~
git clone https://github.com/adligo/pub-keys.adligo.org.git
cd ~/Downloads
sha512sum Apache_OpenOffice_4.1.16_Win_x86_install_en-US.exe > Apache_OpenOffice_4.1.16_Win_x86_install_en-US.exe.sha512
diff Apache_OpenOffice_4.1.16_Win_x86_install_en-US.exe.sha512 ~/pub-keys.adligo.org/pub-keys/net/sourceforge/projects/openofficeorg.mirror/Apache_OpenOffice_4.1.16_Win_x86_install_en-US.exe.sha512
```