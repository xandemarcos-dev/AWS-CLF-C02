---
servico: DynamoDB
dominio: Database
tags: [aws, database, nosql, serverless, clf-c02]
nivel: clf-c02
---

# Amazon DynamoDB

## Em uma frase
> Banco **NoSQL** chave-valor, serverless, com latência de milissegundos em qualquer escala.

## O que é / pra que serve
Banco totalmente gerenciado e serverless para dados não relacionais. Escala automática,
sem servidor para gerenciar. Bom para carrinhos, sessões, perfis, IoT, alta escala.

## Quando usar (e quando NÃO usar)
- ✅ NoSQL, escala massiva, latência baixa e constante, sem gerenciar infra.
- ❌ Dados relacionais com joins complexos / SQL → [[RDS]] ou [[Aurora]].

## Conceitos-chave
- **NoSQL** (chave-valor e documentos).
- **Serverless:** sem provisionar servidores; escala automaticamente.
- Performance de milissegundos consistente em qualquer volume.

## 💰 Modelo de preço
- Paga por capacidade de leitura/escrita (modo provisionado) ou **on-demand** (paga por uso) + armazenamento.

## ⚠️ Pegadinhas de prova
- "NoSQL gerenciado e serverless" → DynamoDB.
- Não é relacional (sem SQL/joins) — isso é [[RDS]]/[[Aurora]].
- Escala automática sem servidor é o grande diferencial citado.

## 🔗 Relacionados
[[RDS]] · [[Aurora]] · [[Lambda]]
