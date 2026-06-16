---
servico: EC2
dominio: Compute
tags: [aws, compute, clf-c02]
nivel: clf-c02
---

# Amazon EC2 (Elastic Compute Cloud)

## Em uma frase
> Servidores virtuais (instâncias) redimensionáveis na nuvem — IaaS.

## O que é / pra que serve
Máquinas virtuais sob demanda. Você escolhe SO, CPU, memória e rede. Controle total
do servidor, com responsabilidade sobre SO e patches ([[Modelo de Responsabilidade Compartilhada]]).

## Quando usar (e quando NÃO usar)
- ✅ Precisa de controle do sistema operacional, software legado, cargas estáveis.
- ❌ Tarefas curtas/event-driven → use [[Lambda]]. Não quer gerenciar servidor → serverless.

## Conceitos-chave
- **Tipos/famílias de instância:** otimizadas para uso geral, compute, memória, etc.
- **AMI:** imagem (template) da instância.
- **Modelos de compra/preço** (ver abaixo).
- Roda dentro de uma [[VPC]]; acesso controlado por **Security Groups**.

## 💰 Modelo de preço
- **On-Demand:** paga por hora/segundo, sem compromisso. Flexível, mais caro.
- **Reserved Instances / Savings Plans:** compromisso de 1–3 anos, grande desconto. Cargas previsíveis.
- **Spot:** capacidade ociosa, até ~90% mais barato, pode ser interrompida. Cargas tolerantes a falha.
- **Dedicated Hosts:** servidor físico dedicado (licenças, compliance).

## ⚠️ Pegadinhas de prova
- **Spot** = mais barato, mas pode ser encerrado a qualquer momento.
- **Reserved/Savings Plans** = economia para uso previsível e contínuo.
- Patch do SO do EC2 é responsabilidade **do cliente**.
- Para escalar automaticamente → **EC2 Auto Scaling** + [[ELB]].

## 🔗 Relacionados
[[Lambda]] · [[Elastic Beanstalk]] · [[EBS]] · [[ELB]] · [[VPC]]
