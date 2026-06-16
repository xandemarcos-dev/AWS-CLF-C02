---
servico: RDS
dominio: Database
tags: [aws, database, clf-c02]
nivel: clf-c02
---

# Amazon RDS (Relational Database Service)

## Em uma frase
> Banco de dados **relacional** gerenciado (MySQL, PostgreSQL, MariaDB, Oracle, SQL Server).

## O que é / pra que serve
A AWS cuida de provisionamento, patches, backups e replicação do banco relacional.
Você foca nos dados e nas queries, não na administração do servidor.

## Quando usar (e quando NÃO usar)
- ✅ Aplicações que precisam de banco SQL/relacional gerenciado.
- ❌ Dados NoSQL/chave-valor com escala massiva → [[DynamoDB]]. Banco em EC2 só se precisar de controle total.

## Conceitos-chave
- **Multi-AZ:** réplica em outra AZ para **alta disponibilidade** (failover automático).
- **Read Replicas:** réplicas de leitura para **escalar performance** de leitura.
- Backups automáticos e snapshots.
- Patch do banco é responsabilidade **da AWS** ([[Modelo de Responsabilidade Compartilhada]]).

## 💰 Modelo de preço
- Paga pela instância de banco (computação), armazenamento e backups.

## ⚠️ Pegadinhas de prova
- **Multi-AZ = disponibilidade** (failover); **Read Replica = performance** de leitura. Não confunda.
- RDS é **relacional**; para NoSQL → [[DynamoDB]].
- Patches do RDS são da AWS (no EC2 seriam do cliente).

## 🔗 Relacionados
[[Aurora]] · [[DynamoDB]] · [[EC2]]
