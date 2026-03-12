# Following Googles Instructions

- [Install Sdk](https://docs.cloud.google.com/sdk/docs/install-sdk#deb)

### Ubuntu Notes

Note the default instructions failed, and I have ammended with these from work with Gemini;

```
mkdir google
cd google
wget -O google.asc https://packages.cloud.google.com/apt/doc/apt-key.gpg
diff google.asc ~/pub-keys.adligo.org/pub-keys/com/google/cloud/packages/apt/doc/2026-02-27.asc
md5sum google.asc > google.asc.md5
diff google.asc.md5 ~/pub-keys.adligo.org/pub-keys/com/google/cloud/packages/apt/doc/2026-02-27.asc.md5

cat google.asc | sudo gpg --dearmor -o /usr/share/keyrings/cloud.google.gpg

echo "deb [signed-by=/usr/share/keyrings/cloud.google.gpg] https://packages.cloud.google.com/apt cloud-sdk main" | sudo tee -a /etc/apt/sources.list.d/google-cloud-sdk.list

sudo apt-get update && sudo apt-get install -y google-cloud-cli
```
