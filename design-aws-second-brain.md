# Design — AWS Second Brain (Vault Obsidian)

**Data:** 2026-06-15
**Autor:** Alexandre + Claude

## Objetivo

Criar uma base de conhecimento de AWS no Obsidian, organizada por **serviço**, que
sirva de fundação para **múltiplas certificações** ao longo do tempo (CLF-C02 agora;
SAA, Developer, etc. no futuro), sem reescrever conteúdo a cada prova.

## Princípio central

- **Serviço** é a unidade reutilizável (uma nota por serviço AWS).
- **Domínio** (Compute, Storage, Security...) é a gaveta/pasta.
- **Certificação** é apenas um índice (Map of Content) que aponta para os serviços
  relevantes, na profundidade exigida. Mesma nota de serviço serve a várias provas.

## Estrutura de pastas

```
AWS-Second-Brain/
├── 00 - Comece aqui.md
├── Certificações/
│   └── CLF-C02.md              (MOC: linka serviços por domínio)
├── Serviços/
│   ├── Compute/   (EC2, Lambda, Elastic Beanstalk, ECS)
│   ├── Storage/   (S3, EBS, EFS)
│   ├── Database/  (RDS, DynamoDB, Aurora)
│   ├── Networking/(VPC, Route 53, CloudFront, ELB)
│   ├── Security/  (IAM, KMS, Shield, WAF)
│   └── Management/(CloudWatch, CloudTrail, Organizations, Cost Explorer)
├── Conceitos/
│   ├── Modelo de Responsabilidade Compartilhada.md
│   ├── Well-Architected Framework.md
│   └── Regiões, AZs e Edge Locations.md
├── Templates/
│   └── _Template Serviço.md
└── _Errei aqui.md
```

## Template de nota de serviço (estrutura fixa)

Frontmatter (`servico`, `dominio`, `tags`, `nivel`) + seções:
Em uma frase · O que é/pra que serve · Quando usar (e quando NÃO) ·
Conceitos-chave · 💰 Modelo de preço · ⚠️ Pegadinhas de prova · 🔗 Relacionados.

As seções "Pegadinhas de prova" e "Quando NÃO usar" são obrigatórias (alto valor
de prova). "🔗 Relacionados" alimenta o grafo do Obsidian.

## Sistema de tags

- Por certificação: `#clf-c02`, futuramente `#saa`, `#dva`.
- Tag base `#aws` + domínio (`#storage`, `#compute`...).
- Permite filtrar "tudo que cai no CLF-C02" num clique.

## Escopo da entrega inicial (CLF-C02)

~20 notas de serviço (núcleo mais cobrado na prova):

| Domínio | Serviços |
|---|---|
| Compute | EC2, Lambda, Elastic Beanstalk, ECS |
| Storage | S3, EBS, EFS |
| Database | RDS, DynamoDB, Aurora |
| Networking | VPC, Route 53, CloudFront, ELB |
| Security | IAM, KMS, Shield, WAF |
| Management | CloudWatch, CloudTrail, Organizations, Cost Explorer |

+ 3 notas de Conceitos (Responsabilidade Compartilhada, Well-Architected,
Regiões/AZs/Edge) + MOC do CLF-C02 + nota de entrada + template + "_Errei aqui".

Demais serviços ficam para o usuário adicionar conforme estuda (template pronto).

## Papel futuro do Claude

Consulta pontual sobre serviços (já coberto pela skill `aws-clf-c02-tutor`).
Claude não mantém o vault no dia a dia — o usuário estuda e preenche.

## Não-objetivos (YAGNI)

- Não cobrir TODOS os serviços AWS de início.
- Não criar conteúdo de SAA/DVA agora (só deixar a arquitetura pronta para isso).
- Não automatizar sync/geração contínua.
