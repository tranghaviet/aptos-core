## Overview

Grafana with preinstall plugins
- yesoreyeram-infinity-datasource

## Setup

Run docker compose

```sh
docker compose up -d
```

## Secure access Grafana

1. Create a Cloudflare Tunnel
1. Add a hostname `your-grafana.your.domain` to `http://grafana:3000` (not `localhost:3000`)

> Note: you don't need to open port `3000` on the server's firewall 😁.

1. Set up Cloudflare WAF to only access from specific IPs
1. **Optional**: Config Grafana OAuth to add make it more secure
