# Guia de Setup e Execução

Este documento explica como configurar e executar o **project-template** em ambiente local, utilizando Docker e Docker Compose.

---

# 📦 Pré-requisitos

Antes de começar, instale:

- Git  
- Docker Desktop (Windows 10/11)  
- Docker Compose (incluso no Docker Desktop)  

---

# 📁 Estrutura Inicial do Projeto

project-template/
├── src/
├── config/
├── infra/docker/
├── scripts/
├── docs/
├── tests/
├── docker-compose.yml
├── docker-compose.override.yml
├── docker-compose.prod.yml
└── .env
---

# 🚀 Rodando o Projeto em Desenvolvimento

O ambiente de desenvolvimento usa:

- `docker-compose.yml`
- `docker-compose.override.yml`

Para subir os containers:

```
docker compose up -d

```

