# QueueOps

Jobs, retries/backoff, observability + panel

## Links
- Live (Vercel): https://dev-kaiki-queueops.vercel.app
- Swagger (Render): https://dev-kaiki-queueops-api.onrender.com/docs
- Health: https://dev-kaiki-queueops-api.onrender.com/health

## One-click deploy

API (Render Blueprint):
https://render.com/deploy?repo=https://github.com/dev-kaiki/queueops

WEB (Vercel):
https://vercel.com/new/clone?repository-url=https://github.com/dev-kaiki/queueops&project-name=dev-kaiki-queueops&repository-name=queueops&root-directory=apps/web

Vercel ENV:
NEXT_PUBLIC_API_URL=https://dev-kaiki-queueops-api.onrender.com

## Local (Windows)
Run:
powershell -ExecutionPolicy Bypass -File .\dev.ps1