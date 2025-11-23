# -------------------------------------------------------
# DOCKERFILE UNIVERSAL TEMPLATE
# Multi-stage + Segurança + Boas Práticas
# -------------------------------------------------------

# ---------- STAGE 1: BUILD ----------
FROM alpine:latest AS builder

# Instala ferramentas comuns usadas em builds
RUN apk update && apk add --no-cache \
    bash \
    curl \
    ca-certificates \
    tzdata \
    build-base

WORKDIR /app

# Copia tudo para o estágio de build
COPY ../../src /app

# Aqui será substituído pelo comando real do seu build futuramente
# Exemplo: npm install; composer install; pip install; go build; etc.
RUN echo "Build stage executado (placeholder)"

# ---------- STAGE 2: RUNTIME ----------
FROM alpine:latest

# Segurança: usuário não-root
RUN addgroup -S appgroup && adduser -S appuser -G appgroup

WORKDIR /app

# Copia arquivos gerados no build
COPY --from=builder /app /app

# Timezone universal
ENV TZ=UTC

# Porta padrão (pode ser alterada no docker-compose)
EXPOSE 8080

# Comando padrão – você mudará isso conforme sua linguagem/framework
CMD ["sh", "-c", "echo 'Template Docker rodando. Configure o CMD real depois.'"]
