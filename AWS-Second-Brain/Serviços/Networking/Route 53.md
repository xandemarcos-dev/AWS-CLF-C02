---
servico: Route 53
dominio: Networking
tags: [aws, networking, dns, clf-c02]
nivel: clf-c02
---

# Amazon Route 53

## Em uma frase
> Serviço de **DNS** gerenciado e registro de domínios da AWS.

## O que é / pra que serve
Traduz nomes de domínio (ex: site.com) em endereços IP, registra domínios e faz
roteamento de tráfego com checagem de saúde. O "53" vem da porta DNS.

## Quando usar (e quando NÃO usar)
- ✅ Gerenciar DNS, registrar domínios, rotear usuários para regiões/recursos.
- ❌ Balancear tráfego dentro de uma região entre instâncias → [[ELB]]. Cache de conteúdo → [[CloudFront]].

## Conceitos-chave
- **DNS gerenciado** + registro de domínios.
- **Health checks:** desvia tráfego se um recurso estiver fora.
- **Políticas de roteamento:** simples, ponderado, latência, geolocalização, failover.

## 💰 Modelo de preço
- Paga por hosted zone e por consultas DNS; registro de domínio à parte.

## ⚠️ Pegadinhas de prova
- "DNS" / "registrar domínio" / "rotear usuários por geografia ou latência" → Route 53.
- DNS (Route 53) ≠ balanceamento dentro da região ([[ELB]]) ≠ CDN ([[CloudFront]]).

## 🔗 Relacionados
[[CloudFront]] · [[ELB]] · [[VPC]]
