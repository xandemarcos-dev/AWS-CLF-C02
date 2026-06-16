---
servico: KMS
dominio: Security
tags: [aws, security, clf-c02]
nivel: clf-c02
---

# AWS KMS (Key Management Service)

## Em uma frase
> Cria e gerencia **chaves de criptografia** para proteger seus dados.

## O que é / pra que serve
Serviço gerenciado para criar, controlar e rotacionar chaves usadas para criptografar
dados em [[S3]], [[EBS]], [[RDS]] e outros. Integra com [[IAM]] para controle de acesso às chaves.

## Quando usar (e quando NÃO usar)
- ✅ Criptografar dados em repouso; gerenciar chaves de forma centralizada e auditável.
- ❌ Controle de acesso/identidade → [[IAM]]. Firewall web → [[WAF]].

## Conceitos-chave
- **Criptografia em repouso** integrada a vários serviços.
- Chaves gerenciadas pela AWS ou pelo cliente; rotação de chaves.
- Uso das chaves é auditado via [[CloudTrail]].

## 💰 Modelo de preço
- Paga por chave gerenciada por mês + número de requisições de API de criptografia.

## ⚠️ Pegadinhas de prova
- "Gerenciar chaves de criptografia" → KMS.
- KMS (criptografia/chaves) ≠ IAM (quem acessa o quê).
- Habilitar criptografia de dados é responsabilidade do cliente.

## 🔗 Relacionados
[[IAM]] · [[S3]] · [[EBS]] · [[CloudTrail]]
