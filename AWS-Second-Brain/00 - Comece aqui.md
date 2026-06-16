---
tags: [aws, indice]
---

# 🧠 AWS Second Brain

Base de conhecimento de AWS organizada por **serviço**, feita para servir a
**várias certificações** ao longo do tempo (CLF-C02 agora; SAA, Developer, etc. depois).

## Como este vault funciona

- **Serviço** é a unidade reutilizável → uma nota por serviço (`[[S3]]`, `[[EC2]]`...).
- **Domínio** é a pasta (Compute, Storage, Security...).
- **Certificação** é só um índice (MOC) que aponta pros serviços que ela cobra.

> Mesma nota de serviço serve a várias provas. Você nunca reescreve sobre o S3.

## Por onde começar

- 🎯 Estudando agora: [[CLF-C02]]
- 📝 Para criar uma nota nova: copie [[_Template Serviço]]
- ⚠️ Pegadinhas que você errou: [[_Errei aqui]]

## Domínios

`Compute` · `Storage` · `Database` · `Networking` · `Security` · `Management`

## Conceitos transversais

- [[Modelo de Responsabilidade Compartilhada]]
- [[Well-Architected Framework]]
- [[Regiões, AZs e Edge Locations]]

## Como adicionar uma certificação futura

1. Crie `Certificações/<NOME>.md` (copie a estrutura do [[CLF-C02]]).
2. Linke os serviços que ela cobra; aprofunde as notas onde precisar.
3. Adicione a tag (`#saa`, `#dva`...) nos serviços relevantes.
