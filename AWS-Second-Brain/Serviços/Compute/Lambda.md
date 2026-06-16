---
servico: Lambda
dominio: Compute
tags: [aws, compute, serverless, clf-c02]
nivel: clf-c02
---

# AWS Lambda

## Em uma frase
> Executa código sem provisionar servidores (serverless) — paga só pela execução.

## O que é / pra que serve
Você sobe uma função; a AWS roda ela em resposta a eventos (upload no [[S3]],
mensagem em fila, requisição de API). Sem servidor para gerenciar, escala automaticamente.

## Quando usar (e quando NÃO usar)
- ✅ Tarefas curtas, event-driven, picos imprevisíveis, microsserviços.
- ❌ Processos longos/contínuos ou que precisam de controle do SO → use [[EC2]].

## Conceitos-chave
- **Event-driven:** dispara por eventos de outros serviços.
- **Escala automática** e sem gerenciamento de infraestrutura.
- Limite de tempo de execução por invocação (curto).

## 💰 Modelo de preço
- Paga por **número de requisições** + **tempo de execução** (GB-segundo).
- **Não paga nada quando não está rodando.** Tem camada gratuita generosa.

## ⚠️ Pegadinhas de prova
- "Sem servidor para gerenciar" + "paga só quando executa" → Lambda.
- Não é para cargas de longa duração.
- É o exemplo clássico de **serverless** na prova.

## 🔗 Relacionados
[[EC2]] · [[S3]] · [[DynamoDB]] · [[CloudWatch]]
