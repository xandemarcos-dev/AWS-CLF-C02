---
servico: EFS
dominio: Storage
tags: [aws, storage, clf-c02]
nivel: clf-c02
---

# Amazon EFS (Elastic File System)

## Em uma frase
> Sistema de **arquivos** compartilhado, montável por várias instâncias [[EC2]] ao mesmo tempo.

## O que é / pra que serve
Armazenamento de arquivos elástico (cresce/encolhe sozinho) acessível por múltiplas
instâncias simultaneamente, inclusive em **várias AZs**. Para Linux (NFS).

## Quando usar (e quando NÃO usar)
- ✅ Vários servidores precisam compartilhar os mesmos arquivos; conteúdo compartilhado.
- ❌ Disco de uma única instância → [[EBS]]. Objetos/backup → [[S3]]. Windows → use FSx.

## Conceitos-chave
- **Compartilhado** entre muitas instâncias e múltiplas AZs.
- **Elástico:** capacidade ajusta automaticamente, paga pelo uso real.
- Protocolo NFS (Linux).

## 💰 Modelo de preço
- Paga pelo **armazenamento realmente usado** (não há provisionamento fixo como no EBS).

## ⚠️ Pegadinhas de prova
- "Vários EC2 acessando os mesmos arquivos ao mesmo tempo" → **EFS**.
- EFS = multi-AZ e compartilhado; EBS = uma AZ e (geralmente) uma instância.
- EFS é para **Linux**; para Windows compartilhado → **Amazon FSx**.

## 🔗 Relacionados
[[EBS]] · [[S3]] · [[EC2]]
