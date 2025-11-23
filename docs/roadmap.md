# Roadmap do Projeto

Este documento apresenta o planejamento de evolução do projeto, incluindo funcionalidades, melhorias, revisões arquiteturais e etapas futuras.

---

## 🟢 Status Atual

- Estrutura inicial do projeto criada
- Pasta `.docker` preparada
- Documentação básica configurada
- Estrutura de contribuição definida
- Arquitetura mapeada

---

## 🟡 Próximas Etapas (Curto Prazo)

### 🔧 1. Configuração completa do Docker
- Criar Dockerfile base
- Criar docker-compose.yml
- Configurar Nginx
- Configurar app  
- Configurar banco de dados  
- Criar volumes e networks  

### 📚 2. Documentação complementar
- Guia de setup local
- Guia de testes
- Guia de deploy

### 🧪 3. Base de testes
- Estrutura inicial para testes automatizados
- Testes de ambiente Docker
- Testes de integração simples

---

## 🔵 Médio Prazo

### ⚙️ 4. Configurar CI/CD
- GitHub Actions (build, tests, lint)
- Deploy automatizado (a definir)
- Pipeline de verificação de segurança

### 🧱 5. Melhorias arquiteturais
- Suporte a múltiplos bancos
- Suporte a múltiplos ambientes (dev/stage/prod)
- Observabilidade (logs, métricas, tracing)

### 🌐 6. Frontend opcional
- Configurar pasta `frontend/`
- Setup com frameworks modernos (React, Vue, Svelte) caso necessário

---

## 🔴 Longo Prazo

### 🛡️ 7. Segurança e robustez
- Harden do Nginx
- Política de CORS avançada
- Compliance (LGPD)

### ☸️ 8. Orquestração
- Preparação para Docker Swarm ou Kubernetes
- Helm charts (futuro)

### 🚀 9. Infraestrutura avançada
- CDN
- Balanceamento de carga
- Escalabilidade horizontal

---

## 📅 Linha do Tempo (Estimativa)

| Etapa | Status | Previsão |
|------|--------|----------|
| Estrutura inicial | ✔️ Concluída | - |
| Configuração Docker | 🔄 Em andamento | Curto prazo |
| CI/CD | ⏳ Pendente | Médio prazo |
| Observabilidade | ⏳ Pendente | Longo prazo |

---

## 📬 Sugestões

Novas ideias são bem-vindas!  
Abra uma issue ou envie um PR com a proposta.
