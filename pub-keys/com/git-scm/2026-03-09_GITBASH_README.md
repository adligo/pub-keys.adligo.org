# Git Bash

### [Download](https://git-scm.com/install/windows)

Download GitBash from here [https://git-scm.com/install/windows](https://git-scm.com/install/windows).

### Compair Check Sums

If you have a previous version of GitBash installed you can run the following shell commands to check the integrity of the file.  This helps ensure someone hasn't hacked the git-scm.com website, or your computer!  Note your version numbers will need to match. 

```
cd ~/Downloads
sha512sum Git-2.53.0-64-bit.exe > Git-2.53.0-64-bit.exe.sha512
diff Git-2.53.0-64-bit.exe.sha512 ~/pub-keys.adligo.org/pub-keys/com/
```

