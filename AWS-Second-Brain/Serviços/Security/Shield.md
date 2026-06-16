---
servico: Shield
dominio: Security
tags: [aws, security, clf-c02]
nivel: clf-c02
---

# AWS Shield

## Em uma frase
> Proteção contra ataques de **DDoS**.

## O que é / pra que serve
Defende aplicações contra ataques de negação de serviço distribuída (DDoS).
**Shield Standard** é automático e gratuito; **Shield Advanced** é pago, com proteção
reforçada e suporte dedicado.

## Quando usar (e quando NÃO usar)
- ✅ Proteger contra DDoS (ataques de volume / inundação de tráfego).
- ❌ Filtrar requisições web maliciosas (SQL injection, XSS) → [[WAF]].

## Conceitos-chave
- **Standard:** ativo por padrão, sem custo, protege contra DDoS comuns.
- **Advanced:** pago, mitigação avançada + acesso ao DDoS Response Team.
- Trabalha junto com [[CloudFront]] e [[Route 53]] na borda.

## 💰 Modelo de preço
- Standard: **gratuito**. Advanced: assinatura mensal + taxas.

## ⚠️ Pegadinhas de prova
- **Shield = DDoS**; **[[WAF]] = filtragem de tráfego web (camada 7)**. Não confunda.
- Shield Standard é automático e grátis para todos.

## 🔗 Relacionados
[[WAF]] · [[CloudFront]] · [[Route 53]]
