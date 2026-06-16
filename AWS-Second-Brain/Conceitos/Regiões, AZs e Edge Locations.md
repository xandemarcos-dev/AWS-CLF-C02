---
tags: [aws, conceito, clf-c02, networking]
nivel: clf-c02
---

# Regiões, AZs e Edge Locations

## Em uma frase
> A infraestrutura global da AWS: Regiões contêm Zonas de Disponibilidade,
> e Edge Locations entregam conteúdo perto do usuário.

## Hierarquia
- **Região (Region):** área geográfica (ex: us-east-1, sa-east-1/São Paulo).
  Isolada das outras. Você escolhe a região por: latência, custo, conformidade/leis, serviços disponíveis.
- **Zona de Disponibilidade (AZ):** um ou mais data centers isolados dentro de uma região.
  Cada região tem **no mínimo 3** AZs. Usar múltiplas AZs = alta disponibilidade.
- **Edge Location:** pontos de presença para cache/entrega de conteúdo (usados pelo
  [[CloudFront]] e Route 53). Muito mais numerosos que as regiões.

## Por que importa
- Distribuir uma aplicação em **múltiplas AZs** protege contra falha de um data center.
- Distribuir em **múltiplas regiões** protege contra falha regional e reduz latência global.

## ⚠️ Pegadinhas de prova
- **Conformidade/soberania de dados** → escolha da **Região**.
- **Alta disponibilidade** → múltiplas **AZs**.
- **Baixa latência para usuários finais (entrega de conteúdo)** → **Edge Locations / CloudFront**.
- Nem todo serviço está em todas as regiões.

## 🔗 Relacionados
[[CloudFront]] · [[Route 53]] · [[EC2]] · [[VPC]]
