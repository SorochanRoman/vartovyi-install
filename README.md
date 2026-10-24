# Vartovyi — installation

Vartovyi watches your Plex watchlist, finds releases with Ukrainian audio on trackers and sends Telegram messages with buttons; after you confirm, the torrent goes to your torrent client.

**Guide:** https://sorochanroman.github.io/vartovyi-install/ ([English](https://sorochanroman.github.io/vartovyi-install/en/guide/) · [Українська](https://sorochanroman.github.io/vartovyi-install/guide/))

| Where | File |
|---|---|
| Synology NAS (DSM 7.2+, Container Manager) | [`docker-compose.yml`](docker-compose.yml) |
| Docker on Linux, Raspberry Pi (64-bit OS) | [`compose.linux.yml`](compose.linux.yml) |

Quick start on Linux:

    mkdir -p ~/vartovyi && cd ~/vartovyi
    curl -fsSL https://raw.githubusercontent.com/SorochanRoman/vartovyi-install/HEAD/compose.linux.yml -o compose.yml
    docker compose up -d

then open `http://<server IP>:8080/setup`. The image `ghcr.io/sorochanroman/vartovyi` is built for amd64 and arm64.

This repository is generated on every release; it is a personal project.

## Українською

Vartovyi стежить за watchlist у Plex, шукає на трекерах роздачі з українською озвучкою і надсилає в Telegram повідомлення з кнопками; після підтвердження торент іде в твій торент-клієнт. Інструкція: https://sorochanroman.github.io/vartovyi-install/guide/ · файли — у таблиці вище.

MIT license.
