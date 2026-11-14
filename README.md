# Whitebeard OS: pacotes prontos

Binários que o instalador do Whitebeard OS baixa, para que quem instala não precise compilar nada nem ter
acesso ao repositório do app, que é privado. O kernel é público: [whitebeard-os](https://github.com/whitebeardit/whitebeard-os).

Cada release traz o arquivo e um `.sha256`. O kernel fixa URL e sha256 em `kernel/versions.env` e recusa
qualquer arquivo cujo sha256 não confira.

| release | o que é |
|---|---|
| `jarvis-web-<versão>` | JARVIS Web pronto (UI construída + servidor), um pacote para macOS e Linux |
| `ffmpeg-whisper-metal-<versão>-darwin-arm64` | FFmpeg LGPL com whisper.cpp na GPU (Metal) e avfoundation (câmera/microfone) |
| `ffmpeg-whisper-cpu-<versão>-linux-x86_64` | FFmpeg LGPL estático com whisper.cpp em CPU |
| `kit-divulgacao-<data>` | kit de divulgação: prints, vídeos e GIFs do Whitebeard OS |

## Licença

O pacote do JARVIS Web e o kit de divulgação seguem a [Whitebeard OS Personal Use License](LICENSE): **grátis para
uso pessoal; uso comercial exige licença**, em [whitebeard.dev](https://whitebeard.dev). Os builds do FFmpeg são
software de terceiros e seguem a licença do FFmpeg (LGPL), não a nossa.
