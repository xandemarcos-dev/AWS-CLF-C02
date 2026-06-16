---
servico: Elastic Beanstalk
dominio: Compute
tags: [aws, compute, clf-c02]
nivel: clf-c02
---

# AWS Elastic Beanstalk

## Em uma frase
> Suba seu código e a AWS provisiona e gerencia a infraestrutura (PaaS) automaticamente.

## O que é / pra que serve
Plataforma que cuida de provisionamento de [[EC2]], balanceamento ([[ELB]]),
auto scaling e monitoramento para você. Você foca no código da aplicação.

## Quando usar (e quando NÃO usar)
- ✅ Quer fazer deploy de uma app web sem montar a infraestrutura na mão.
- ❌ Precisa de controle fino da infra → monte direto com [[EC2]]/[[VPC]].

## Conceitos-chave
- Você ainda **tem acesso** aos recursos subjacentes (EC2, etc.) e mantém controle.
- Suporta várias linguagens/plataformas (Java, .NET, Node, Python...).
- **Não cobra pelo serviço** — você paga só os recursos que ele cria.

## 💰 Modelo de preço
- O Beanstalk em si é **gratuito**; paga pelos recursos provisionados (EC2, S3, etc.).

## ⚠️ Pegadinhas de prova
- "Deploy fácil de aplicação, AWS gerencia a infra, mas mantenho controle" → Beanstalk.
- Diferente de [[Lambda]]: aqui ainda há servidores (EC2) por baixo.
- O serviço é grátis; só os recursos custam.

## 🔗 Relacionados
[[EC2]] · [[ELB]] · [[Lambda]]
