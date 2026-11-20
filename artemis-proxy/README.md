# Artemis Proxy

Artemis Proxy is a streaming transport backend for browser-side web proxy engines, with a clean modern frontend.

## Features

- Fast streaming proxy with HTML/CSS/JS rewriting
- Built-in ad blocker
- WebSocket & Wisp transport support
- Account-friendly (GitHub and more)
- Polished landing page UI

## Install

```bash
npm install
```

Requires **Node.js 24.x**.

## Run

```bash
npm start
```

Server listens on port `8080` by default (or `PORT` env var).

Open: **http://localhost:8080/**

## Proxy endpoint

```
/artemis?url=https://example.com/
```

Example:

```
http://localhost:8080/artemis?url=https://example.com/
```

## Frontend

The root path `/` serves the included `index.html` landing page.  
You can customize the endpoint in the page's config script if needed.

## Configuration

| Variable | Default | Description |
|----------|---------|-------------|
| `PORT` | `8080` | Listen port |
| `PROXY_ENDPOINT` | `/artemis?url=` | Proxy path + query prefix |
| `WISP_PATH` | `/wisp/` | Wisp transport path |
| `REWRITE` | `true` | Enable content rewriting |
| `ALLOW_PRIVATE_TARGETS` | `false` | Allow private/LAN targets |
| `UPSTREAM_TIMEOUT` | `30000` | Upstream timeout (ms) |
| `MAX_REDIRECTS` | `8` | Max redirect hops |

See `HELP.md` for more.

## License

Open source. Use it for your own proxies — just don't claim the original work as yours.
