# Ollama Open Claw

- [Download for Windows](https://ollama.com/download)

```
cd ~/Downloads
curl https://ollama.com/download/OllamaSetup.exe
sha512sum OllamaSetup.exe > OllamaSetup.exe.sha512
cat OllamaSetup.exe.sha512
diff OllamaSetup.exe.sha512 ~/pub-keys.adligo.org/pub-keys/com/ollama/download/OllamaSetup.exe.sha512
```
