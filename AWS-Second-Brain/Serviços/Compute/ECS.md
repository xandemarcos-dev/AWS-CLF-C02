---
servico: ECS
dominio: Compute
tags: [aws, compute, containers, clf-c02]
nivel: clf-c02
---

# Amazon ECS (Elastic Container Service)

## Em uma frase
> Orquestra contêineres (Docker) na AWS.

## O que é / pra que serve
Serviço gerenciado para rodar e escalar aplicações em contêineres. Pode rodar sobre
[[EC2]] (você gerencia os servidores) ou com **Fargate** (serverless, sem gerenciar servidor).

## Quando usar (e quando NÃO usar)
- ✅ Sua aplicação é containerizada (Docker) e precisa de orquestração.
- ❌ Função única event-driven simples → [[Lambda]]. App monolítica simples → [[Elastic Beanstalk]].

## Conceitos-chave
- **Contêiner:** empacota app + dependências de forma portável.
- **Fargate:** modo serverless do ECS (sem gerenciar EC2).
- **EKS:** alternativa baseada em Kubernetes (cite-se na prova como "Kubernetes gerenciado").

## 💰 Modelo de preço
- Com EC2: paga as instâncias EC2. Com **Fargate**: paga vCPU/memória usados pela tarefa.

## ⚠️ Pegadinhas de prova
- "Rodar contêineres Docker" → ECS (ou EKS para Kubernetes).
- **Fargate** = contêineres **sem** gerenciar servidores.
- **EKS** = Kubernetes gerenciado.

## 🔗 Relacionados
[[EC2]] · [[Lambda]]
