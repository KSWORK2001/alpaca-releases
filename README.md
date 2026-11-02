<div align="center">

# 🦙 Alpaca

**A local model runtime for Apple Silicon — sort of like Ollama, but better.**

Web UI · OpenAI + Ollama APIs · web search · runtime model switching · SSD-offloaded MoE playground

**⬇️ [Download the latest release below](https://github.com/KSWORK2001/alpaca-releases/releases/latest)**

</div>

---

## Install (macOS, Apple Silicon, Python 3.12+)

```bash
curl -fsSL https://github.com/KSWORK2001/alpaca-releases/releases/latest/download/install.sh | bash
```

Then:

```bash
alpaca serve                 # start the runtime
open http://127.0.0.1:8080   # chat UI, settings, model manager
```

Upgrading an existing install: `alpaca update --apply`

## What's inside each release

| Asset | What it is |
|---|---|
| `alpaca-vX.Y.Z.tar.gz` | The full runtime: gateway, web UI, CLI, install scripts |
| `install.sh` | The one-line installer above |
| `latest.json` | Auto-update feed consumed by `alpaca update` |
| `SHA256SUMS` | Checksums for the tarball |

## Release feed (for tooling)

```bash
curl -fsSL https://github.com/KSWORK2001/alpaca-releases/releases/latest/download/latest.json
```

## Security notes

The runtime binds to `127.0.0.1` by default and generates a local API key on
first run. Models you download are your responsibility — Alpaca runs whatever
open-weight models you give it, including uncensored research builds.
