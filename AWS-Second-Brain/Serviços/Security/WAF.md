---
servico: WAF
dominio: Security
tags: [aws, security, clf-c02]
nivel: clf-c02
---

# AWS WAF (Web Application Firewall)

## Em uma frase
> Firewall de aplicação web que filtra requisições maliciosas (camada 7).

## O que é / pra que serve
Cria regras para bloquear tráfego web malicioso — SQL injection, cross-site scripting (XSS),
bots, IPs específicos. Protege apps expostas via [[CloudFront]] ou [[ELB]].

## Quando usar (e quando NÃO usar)
- ✅ Bloquear ataques na camada de aplicação (HTTP/HTTPS); filtrar por regras.
- ❌ Ataques de volume/DDoS → [[Shield]]. Identidade/acesso → [[IAM]].

## Conceitos-chave
- Regras configuráveis (allow/block) por padrões, IP, geografia, rate limit.
- Atua na **camada 7** (aplicação web).
- Integra com [[CloudFront]], [[ELB]] (ALB) e API Gateway.

## 💰 Modelo de preço
- Paga por web ACL, por regra e por número de requisições inspecionadas.

## ⚠️ Pegadinhas de prova
- **WAF = filtra requisições web (SQL injection, XSS, camada 7)**; **[[Shield]] = DDoS**.
- WAF e Shield costumam aparecer juntos como complementares.

## 🔗 Relacionados
[[Shield]] · [[CloudFront]] · [[ELB]]
