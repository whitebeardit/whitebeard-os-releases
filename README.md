# Whitebeard OS: pacotes prontos

Binários que o instalador do Whitebeard OS baixa, para que quem instala não precise compilar nada nem ter
acesso aos repositórios de código (que são privados).

Cada release traz o arquivo e um `.sha256`. O kernel fixa URL e sha256 em `kernel/versions.env` e recusa
qualquer arquivo cujo sha256 não confira.

| release | o que é |
|---|---|
| `jarvis-web-<versão>` | JARVIS Web pronto (UI construída + servidor), um pacote para macOS e Linux |
| `ffmpeg-whisper-metal-<versão>-darwin-arm64` | FFmpeg LGPL com whisper.cpp na GPU (Metal) e avfoundation (câmera/microfone) |
| `ffmpeg-whisper-cpu-<versão>-linux-x86_64` | FFmpeg LGPL estático com whisper.cpp em CPU |
