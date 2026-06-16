---
tags: [aws, conceito, clf-c02, security]
nivel: clf-c02
---

# Modelo de Responsabilidade Compartilhada

## Em uma frase
> A AWS é responsável pela segurança **DA** nuvem; você é responsável pela segurança **NA** nuvem.

## A divisão
- **AWS (Security OF the cloud):** hardware, rede física, data centers,
  virtualização, infraestrutura dos serviços gerenciados.
- **Cliente (Security IN the cloud):** seus dados, configuração de IAM,
  criptografia, patches do SO (em EC2), regras de firewall/Security Groups,
  configuração das aplicações.

## A linha se move conforme o serviço
- **EC2 (IaaS):** você cuida de mais (SO, patches, rede). Mais controle, mais responsabilidade.
- **RDS / Lambda (PaaS/serverless):** AWS cuida do SO e patches do serviço; você cuida
  de dados, acesso e config.
- **S3 (gerenciado):** AWS cuida da infra; você cuida de quem acessa e da criptografia.

## ⚠️ Pegadinhas de prova
- Patch do **sistema operacional do EC2** é responsabilidade **do cliente**.
- Patch do banco no **RDS** é responsabilidade **da AWS**.
- Segurança **física** dos data centers é **sempre** da AWS.
- Configuração de IAM e dados são **sempre** do cliente.

## 🔗 Relacionados
[[IAM]] · [[EC2]] · [[RDS]] · [[Well-Architected Framework]]
