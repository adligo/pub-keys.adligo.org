# VS Code Install

# [Download](https://code.visualstudio.com/)

Download VS code from here [https://code.visualstudio.com/](https://code.visualstudio.com/).

# [Download and Install GitBash](../../git-scm/install/2026-03-09_GITBASH_README.md)

# [Download pub-keys.adligo.org](../../../README.md)

Run the following Bash commands in GitBash to check the integrity of the file.  This helps ensure someone hasn't hacked the git-scm.com website, or your computer!  Note your version numbers will need to match. 

```
cd ~/Downloads
sha512sum VSCodeUserSetup-x64-1.111.0.exe > VSCodeUserSetup-x64-1.111.0.exe.sha512
diff VSCodeUserSetup-x64-1.111.0.exe.sha512  ~/pub-keys.adligo.org/pub-keys/com/visualstudio/code/VSCodeUserSetup-x64-1.111.0.exe.sha512
```