---
servico: ELB
dominio: Networking
tags: [aws, networking, clf-c02]
nivel: clf-c02
---

# Elastic Load Balancing (ELB)

## Em uma frase
> Distribui o tráfego de entrada entre várias instâncias/AZs para alta disponibilidade.

## O que é / pra que serve
Recebe as requisições e as reparte entre múltiplos alvos (ex: [[EC2]]) em várias AZs.
Se um alvo cai, desvia para os saudáveis. Base de aplicações resilientes e escaláveis.

## Quando usar (e quando NÃO usar)
- ✅ Distribuir carga entre instâncias; alta disponibilidade dentro de uma região.
- ❌ DNS/roteamento global → [[Route 53]]. CDN → [[CloudFront]].

## Conceitos-chave
- Trabalha junto com **Auto Scaling** para escalar a frota.
- **Health checks:** só envia tráfego para alvos saudáveis.
- Tipos: **ALB** (HTTP/HTTPS, camada 7), **NLB** (camada 4, alto desempenho), GLB.

## 💰 Modelo de preço
- Paga por hora do load balancer + unidades de capacidade processadas.

## ⚠️ Pegadinhas de prova
- "Distribuir tráfego entre instâncias / entre AZs" → ELB.
- ELB (balanceia na região) ≠ Route 53 (DNS) ≠ CloudFront (CDN).
- **ALB = HTTP/HTTPS (camada 7)**; **NLB = camada 4** (TCP, ultra performance).

## 🔗 Relacionados
[[EC2]] · [[Route 53]] · [[VPC]]
