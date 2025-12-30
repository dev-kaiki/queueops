<div align="center">

# queueops

<a href="https://dev-kaiki-queueops.vercel.app"><img src="https://img.shields.io/badge/LIVE%20DEMO-Vercel-111?style=for-the-badge&logo=vercel&logoColor=white"></a>
<a href="https://dev-kaiki-queueops-api.onrender.com/docs"><img src="https://img.shields.io/badge/SWAGGER-API%20Docs-111?style=for-the-badge&logo=swagger&logoColor=white"></a>
<a href="https://github.com/dev-kaiki/queueops"><img src="https://img.shields.io/badge/REPO-GitHub-111?style=for-the-badge&logo=github&logoColor=white"></a>

</div>

## Quick Links
- Live: https://dev-kaiki-queueops.vercel.app
- Swagger: https://dev-kaiki-queueops-api.onrender.com/docs

## Deploy (1-click)
- Deploy API (Render): https://render.com/deploy?repo=https://github.com/dev-kaiki/queueops
- Deploy Web (Vercel): https://vercel.com/new/clone?repository-url=https://github.com/dev-kaiki/queueops

---

# QueueOps â€” Jobs + Retries/Backoff + Monitoring (BullMQ + Redis)

[![CI](https://github.com/dev-kaiki/queueops/actions/workflows/ci.yml/badge.svg)](https://github.com/dev-kaiki/queueops/actions/workflows/ci.yml)
![Node](https://img.shields.io/badge/node-20%2B-222?logo=node.js)
![NestJS](https://img.shields.io/badge/nestjs-10-222?logo=nestjs)
![Redis](https://img.shields.io/badge/redis-7-222?logo=redis)
![Docker](https://img.shields.io/badge/docker-ready-222?logo=docker)

Demo focado em **confiabilidade**: filas, retries, backoff, dead-letter e painel simples de monitoramento.

> **Status atual:** repo criado a partir do template (API + Web + Redis no docker-compose).  
> Endpoints prontos: `/health`, `/users` e Swagger `/docs`.  
> A fila BullMQ entra no roadmap abaixo.

---

## ðŸŽ¯ Objetivo
Simular cenÃ¡rios reais:
- jobs que falham e se recuperam (retries)
- backoff exponencial
- DLQ (dead-letter queue)
- observabilidade bÃ¡sica (status/tempo)

---

## âœ… Roadmap (MVP do demo)
- [ ] BullMQ + workers
- [ ] Jobs: `sendEmail`, `generatePdf`, `syncData`
- [ ] Retries + backoff + timeout
- [ ] DLQ (falhas permanentes)
- [ ] Tela Web: lista de jobs + status + reprocessar

---

## â–¶ï¸ Rodar local
```powershell
corepack enable
corepack prepare pnpm@latest --activate

pnpm install
docker compose up -d

