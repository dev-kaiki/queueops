# QueueOps — Jobs + Retries/Backoff + Monitoring (BullMQ + Redis)

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

## 🎯 Objetivo
Simular cenários reais:
- jobs que falham e se recuperam (retries)
- backoff exponencial
- DLQ (dead-letter queue)
- observabilidade básica (status/tempo)

---

## ✅ Roadmap (MVP do demo)
- [ ] BullMQ + workers
- [ ] Jobs: `sendEmail`, `generatePdf`, `syncData`
- [ ] Retries + backoff + timeout
- [ ] DLQ (falhas permanentes)
- [ ] Tela Web: lista de jobs + status + reprocessar

---

## ▶️ Rodar local
```powershell
corepack enable
corepack prepare pnpm@latest --activate

pnpm install
docker compose up -d
