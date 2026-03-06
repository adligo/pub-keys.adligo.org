# Official Dot Net Download Site

https://dotnet.microsoft.com/en-us/download/visual-studio-sdks?cid=msbuild-developerpacks

```
cd Downloads
wget https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/sdk-10.0.103-windows-x64-installer
sha512sum dotnet-sdk-10.0.103-win-x64.exe > dotnet-sdk-10.0.103-win-x64.exe.sha512
diff dotnet-sdk-10.0.103-win-x64.exe.sha512 ~/pub-keys.adligo.org/pub-keys/com/microsoft/dotnet/en-us/download/dotnet/thank-you/dotnet-sdk-10.0.103-win-x64.exe.sha512

```