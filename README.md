# Kelo server

The server of [Kelo](https://kelo.chat), the AI assistant that runs on a server you set up. This repository holds only what the
server needs to install and run, taken from each release of the full source at
[github.com/kelo-chat/kelo](https://github.com/kelo-chat/kelo) (apps, server and docs). Each commit here is one release, with
the same `release-<version>` tag as there.

## Install

macOS and Linux:

```sh
curl -fsSL https://kelo.chat/install.sh | bash
```

Windows (PowerShell):

```powershell
irm https://kelo.chat/install.ps1 | iex
```

The installer checks Docker, gets `uv` if it is missing, puts these files in `~/kelo` and opens the guided setup. Then scan the
server's QR code with the Kelo app. By hand: `git clone https://github.com/kelo-chat/kelo-server kelo && cd kelo && uv run assistant setup`.

Install guide: [kelo.chat/install](https://kelo.chat/install) · [docs/install.md](docs/install.md)

Server size: minimum 2 GB RAM · 2 CPU cores · 10 GB free disk; recommended 4 GB · 4 cores · 20 GB.

Signed release images: `ghcr.io/kelo-chat/server`, `ghcr.io/kelo-chat/workroom`, `ghcr.io/kelo-chat/updater`.

## 설치 (한국어)

macOS·Linux는 `curl -fsSL https://kelo.chat/install.sh | bash`, Windows는 PowerShell에서 `irm https://kelo.chat/install.ps1 | iex`.
설치 스크립트가 Docker를 확인하고, 없으면 uv를 설치하고, 이 파일들을 `~/kelo`에 넣은 뒤 설정 화면을 열어요. 설치 안내: [kelo.chat/install](https://kelo.chat/install)

## License

AGPL-3.0 (see [LICENSE](LICENSE) and [NOTICE](NOTICE)). Issues and the full source: [kelo-chat/kelo](https://github.com/kelo-chat/kelo).
