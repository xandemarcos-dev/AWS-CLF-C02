---
servico: Aurora
dominio: Database
tags: [aws, database, clf-c02]
nivel: clf-c02
---

# Amazon Aurora

## Em uma frase
> Banco relacional da AWS compatível com **MySQL e PostgreSQL**, mais rápido e gerenciado.

## O que é / pra que serve
Engine de banco relacional próprio da AWS, parte do [[RDS]], com desempenho superior
(até ~5x MySQL / ~3x PostgreSQL), replicação e recuperação automáticas.

## Quando usar (e quando NÃO usar)
- ✅ Quer um relacional gerenciado de alto desempenho compatível com MySQL/PostgreSQL.
- ❌ NoSQL/escala chave-valor → [[DynamoDB]]. Precisa de engine específico (Oracle/SQL Server) → [[RDS]].

## Conceitos-chave
- Compatível com **MySQL e PostgreSQL**.
- Armazenamento replicado em **várias AZs** automaticamente; tolerante a falhas.
- **Aurora Serverless:** escala a capacidade conforme a demanda.

## 💰 Modelo de preço
- Paga pela capacidade de computação + armazenamento (cresce automaticamente). Serverless paga por uso.

## ⚠️ Pegadinhas de prova
- "Compatível com MySQL/PostgreSQL, mas mais rápido e da própria AWS" → Aurora.
- Faz parte do RDS, mas é o engine premium.
- Continua sendo **relacional** (não confundir com DynamoDB).

## 🔗 Relacionados
[[RDS]] · [[DynamoDB]]
