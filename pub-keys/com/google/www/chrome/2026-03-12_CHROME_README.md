# Google Chrome

- [https://www.google.com/chrome/dr/download](https://www.google.com/chrome/dr/download)

```
cd ~/Downloads
sha512sum google-chrome-stable_current_amd64.deb > google-chrome-stable_current_amd64.deb.sha512

cat google-chrome-stable_current_amd64.deb.sha512 

diff google-chrome-stable_current_amd64.deb.sha512 ~/pub-keys.adligo.org/pub-keys/com/google/www/chrome/dr/download/google-chrome-stable_current_amd64.deb.sha512

```
