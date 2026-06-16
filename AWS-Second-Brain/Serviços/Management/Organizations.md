---
servico: Organizations
dominio: Management
tags: [aws, management, billing, clf-c02]
nivel: clf-c02
---

# AWS Organizations

## Em uma frase
> Gerencia **várias contas AWS** de forma central, com faturamento consolidado e políticas.

## O que é / pra que serve
Agrupa múltiplas contas sob uma organização: cobrança unificada, descontos por volume,
e políticas de controle (**SCPs**) que limitam o que cada conta pode fazer.

## Quando usar (e quando NÃO usar)
- ✅ Empresa com várias contas (por time/ambiente); governança e billing central.
- ❌ Controlar permissões **dentro** de uma conta → [[IAM]].

## Conceitos-chave
- **Faturamento consolidado:** uma fatura para todas as contas + descontos por volume agregado.
- **OUs (Organizational Units):** agrupam contas.
- **SCPs (Service Control Policies):** definem o teto de permissões das contas.

## 💰 Modelo de preço
- O serviço é **gratuito**; o benefício é consolidar custos e ganhar descontos por volume.

## ⚠️ Pegadinhas de prova
- "Gerenciar várias contas" / "fatura consolidada" / "desconto por volume" → Organizations.
- **SCP** limita o que a conta pode fazer (teto), mas não concede permissão (isso é o [[IAM]]).

## 🔗 Relacionados
[[IAM]] · [[Cost Explorer]] · [[CloudTrail]]
