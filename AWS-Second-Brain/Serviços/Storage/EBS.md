---
servico: EBS
dominio: Storage
tags: [aws, storage, clf-c02]
nivel: clf-c02
---

# Amazon EBS (Elastic Block Store)

## Em uma frase
> Disco de **bloco** persistente para anexar a uma instância [[EC2]].

## O que é / pra que serve
Volume de armazenamento (como um HD/SSD) que você anexa a uma instância EC2.
Persiste mesmo se a instância for parada. Bom para SO, bancos e arquivos da aplicação.

## Quando usar (e quando NÃO usar)
- ✅ Disco para uma instância EC2; banco de dados que precisa de baixa latência.
- ❌ Vários servidores acessando ao mesmo tempo → [[EFS]]. Objetos/arquivos web → [[S3]].

## Conceitos-chave
- **Armazenamento de bloco**, anexado a **uma** instância (geralmente na mesma AZ).
- **Snapshots:** backups incrementais armazenados no [[S3]].
- Tipos: SSD (desempenho) e HDD (throughput/custo).

## 💰 Modelo de preço
- Paga pelo **tamanho provisionado** (GB) do volume, independente do uso, + IOPS em alguns tipos.

## ⚠️ Pegadinhas de prova
- EBS = bloco, **1 instância por vez** (em geral); EFS = arquivo, **muitas** instâncias.
- Volume é **preso a uma AZ**; snapshot vai pro S3 e permite recriar em outra AZ.
- Persiste após parar a instância (diferente de instance store).

## 🔗 Relacionados
[[EC2]] · [[S3]] · [[EFS]]
