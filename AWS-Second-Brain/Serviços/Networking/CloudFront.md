---
servico: CloudFront
dominio: Networking
tags: [aws, networking, cdn, clf-c02]
nivel: clf-c02
---

# Amazon CloudFront

## Em uma frase
> **CDN** (rede de entrega de conteúdo) que faz cache perto do usuário nas Edge Locations.

## O que é / pra que serve
Distribui conteúdo (sites, vídeos, APIs, arquivos do [[S3]]) a partir de
[[Regiões, AZs e Edge Locations|Edge Locations]], reduzindo latência e carga na origem.

## Quando usar (e quando NÃO usar)
- ✅ Entregar conteúdo rápido a usuários globais; reduzir latência; proteger origem.
- ❌ DNS → [[Route 53]]. Balanceamento interno → [[ELB]]. Armazenamento → [[S3]].

## Conceitos-chave
- **Cache em Edge Locations** próximas do usuário final.
- Integra com [[S3]] e outras origens.
- Pode integrar com [[WAF]] e [[Shield]] para segurança na borda.

## 💰 Modelo de preço
- Paga por transferência de dados de saída e número de requisições nas edge locations.

## ⚠️ Pegadinhas de prova
- "Reduzir latência entregando conteúdo perto do usuário" / "CDN" → CloudFront.
- Usa **Edge Locations** (não AZs).
- Não confundir com Route 53 (DNS) nem ELB (balanceamento na região).

## 🔗 Relacionados
[[S3]] · [[Route 53]] · [[WAF]] · [[Shield]] · [[Regiões, AZs e Edge Locations]]
