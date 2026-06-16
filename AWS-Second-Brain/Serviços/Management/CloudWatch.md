---
servico: CloudWatch
dominio: Management
tags: [aws, management, clf-c02]
nivel: clf-c02
---

# Amazon CloudWatch

## Em uma frase
> **Monitoramento** de métricas, logs e alarmes dos recursos AWS.

## O que é / pra que serve
Coleta métricas (CPU, rede, etc.), centraliza logs e dispara **alarmes** e ações
automáticas (ex: acionar Auto Scaling). Responde "como meus recursos estão se saindo?".

## Quando usar (e quando NÃO usar)
- ✅ Monitorar desempenho, criar alarmes, observar logs, gatilhos de automação.
- ❌ Auditar **quem fez o quê** na conta → [[CloudTrail]].

## Conceitos-chave
- **Métricas** (desempenho) e **Logs** centralizados.
- **Alarmes:** notificam (via SNS) ou agem quando um limite é cruzado.
- **Dashboards** de visualização.

## 💰 Modelo de preço
- Paga por métricas personalizadas, logs ingeridos/armazenados, alarmes e dashboards.

## ⚠️ Pegadinhas de prova
- **CloudWatch = desempenho/monitoramento** ("o quê/como"); **[[CloudTrail]] = auditoria** ("quem fez").
- Alarme de CloudWatch pode disparar **Auto Scaling**.

## 🔗 Relacionados
[[CloudTrail]] · [[EC2]] · [[Lambda]] · [[Well-Architected Framework]]
