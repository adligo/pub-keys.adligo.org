# WordPress

```
cd ~/Downloads
wget https://wordpress.org/latest.zip
sha512sum wordpress-6.9.4.zip > wordpress-6.9.4.zip.sha512
diff wordpress-6.9.4.zip.sha512 ~/pub-keys.adligo.org/pub-keys/org/wordpress/download/wordpress-6.9.4.zip.sha512
```