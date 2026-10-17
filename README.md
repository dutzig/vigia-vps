# vigia-vps

External watchdog: every 10 minutes GitHub Actions tests whether the VPS answers (TCP connection), and sends a Telegram message when it goes down and when it comes back. It exists because every alert of the bots runs inside the VPS itself; if the VPS goes down, those alerts go down with it.

Secrets (never in the code): `VPS_ALVO`, `TG_TOKEN`, `TG_CHAT`.
