# Eclipse

Download from a mirror

- [Eclipse IDE Download site](https://eclipseide.org/)

```
cd ~/Downloads
sha512sum eclipse-inst-jre-win64.exe > eclipse-inst-jre-win64.exe.sha512
cat eclipse-inst-jre-win64.exe.sha512
diff eclipse-inst-jre-win64.exe.sha512 ~/pub-keys.adligo.org/pub-keys/org/eclipse/www/downloads/eclipse-inst-jre-win64.exe.sha512
```