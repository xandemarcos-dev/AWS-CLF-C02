---
servico: CloudTrail
dominio: Management
tags: [aws, management, security, clf-c02]
nivel: clf-c02
---

# AWS CloudTrail

## Em uma frase
> **Auditoria:** registra quem fez o quê na conta (chamadas de API).

## O que é / pra que serve
Grava um histórico de todas as ações/chamadas de API feitas na conta — por quem, quando,
de onde. Essencial para auditoria, conformidade e investigação de incidentes.

## Quando usar (e quando NÃO usar)
- ✅ Saber **quem** criou/alterou/excluiu um recurso; trilha de auditoria; compliance.
- ❌ Medir **desempenho** / métricas / logs de aplicação → [[CloudWatch]].

## Conceitos-chave
- Registra **chamadas de API** (console, CLI, SDK).
- Logs podem ser entregues a um bucket [[S3]] para retenção.
- Ajuda em **governança e conformidade**.

## 💰 Modelo de preço
- Histórico de eventos recentes é gratuito; trilhas adicionais e armazenamento no S3 custam.

## ⚠️ Pegadinhas de prova
- **CloudTrail = quem fez o quê (auditoria)**; **[[CloudWatch]] = como está se saindo (desempenho)**.
  Esta é uma das distinções mais cobradas no CLF-C02.

## 🔗 Relacionados
[[CloudWatch]] · [[IAM]] · [[S3]] · [[Organizations]]
