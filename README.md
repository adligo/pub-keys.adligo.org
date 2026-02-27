# pub-keys.adligo.org

Although this project is far from a Certificate Authority, it serves a similar purpose by tracking various public keys that are used in code signing from various sources.

# pub-keys directory

I have stored the public keys in various formats as I install software that uses the PGP Web of Trust under there Java style domain spaces.  For example, I started today with Hashicorp's terriform install instructions;

-[https://developer.hashicorp.com/terraform/install](https://developer.hashicorp.com/terraform/install)

Saving the file to this project with this command;

```
  wget -O com/hashicorp/releases/apt/2026-02-27.asc https://apt.releases.hashicorp.com/gpg
```

You can now see if you get a different public key from Hashicorp in the future by doing a diff of your copy of the file before you add it to your PGP keyring and trust the code it signed.  For Example;

```
  git clone https://github.com/adligo/pub-keys.adligo.org.git
  wget -O latest-hashicorp.asc https://apt.releases.hashicorp.com/gpg
  # No differences should exist, if they do either hashicorp changed it's key or got hacked
  diff latest-hashicorp.asc pub-keys.adligo.org/pub-keys/com/hashicorp/releases/apt/2026-02-27.asc
  # Alternative check 
  md5sum latest-hashicorp.asc > latest-hashicorp.asc.md5
  cat latest-hashicorp.asc.md5
  # These should have different file names but the same md5 checksum
  diff latest-hashicorp.asc.md5 pub-keys.adligo.org/pub-keys/com/hashicorp/releases/apt/2026-02-27.asc.md5
```

Currently most code signing certificates rotate every 15 months (460 days);

- [https://www.digicert.com/blog/understanding-the-new-code-signing-certificate-validity-change](https://www.digicert.com/blog/understanding-the-new-code-signing-certificate-validity-change)
- [https://www.ssl.com/article/reminder-reduced-code-signing-certificate-lifecycles/](https://www.ssl.com/article/reminder-reduced-code-signing-certificate-lifecycles/)
- [https://www.globalsign.com/en/blog/code-signing-validity-changes](https://www.globalsign.com/en/blog/code-signing-validity-changes)

