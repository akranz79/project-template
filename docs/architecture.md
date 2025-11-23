# Arquitetura do Projeto

Este documento descreve a visão geral da arquitetura do projeto **project-template**.

## Objetivo

Fornecer um esqueleto base para qualquer aplicação real, independente da linguagem ou framework, contendo:

- Estrutura de pastas profissional
- Dockerfile multi-stage
- Composes para desenvolvimento e produção
- Pipeline CI/CD em GitHub Actions
- Arquivos de documentação padrão

## Componentes Principais

### 1. **Aplicação (`src/`)**
Contém o código-fonte da aplicação (independente da stack).

### 2. **Infraestrutura (`infra/`)**
Contém arquivos relacionados à infraestrutura, como:
- Dockerfile
- Configurações de containers
- Configurações de build

### 3. **Config (`config/`)**
Futuras configurações de ambiente, runtime, ou providers.

### 4. **Scripts (`scripts/`)**
Contém scripts CLI para automações (build, setup, deploy).

### 5. **Documentação (`docs/`)**
Guia para arquitetura, setup e contribuição.

## Fluxo de Deploy

1. Push na branch `main`
2. Pipeline do GitHub Actions executa:
   - Build
   - Testes
   - Lint/Security
   - Docker build
3. (Opcional) Push para GHCR

## Arquitetura do Docker

O template usa:
- Multi-stage para reduzir tamanho da imagem
- Usuário não-root
- Override para dev
- Compose separado para produção
- Healthcheck
- Rotação de logs

---

Este documento pode ser expandido conforme o projeto evoluir.
