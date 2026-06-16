---
servico: IAM
dominio: Security
tags: [aws, security, clf-c02]
nivel: clf-c02
---

# AWS IAM (Identity and Access Management)

## Em uma frase
> Controla **quem** pode fazer **o quê** na sua conta AWS.

## O que é / pra que serve
Gerencia identidades (usuários, grupos, funções) e permissões (políticas) para acessar
recursos AWS. É a base da segurança da conta. Gratuito.

## Quando usar (e quando NÃO usar)
- ✅ Sempre — controle de acesso, MFA, permissões mínimas (least privilege).
- ❌ Criptografia de dados → [[KMS]]. Proteção web/DDoS → [[WAF]]/[[Shield]].

## Conceitos-chave
- **Usuário** (pessoa/serviço), **Grupo** (conjunto de usuários), **Role/Função**
  (permissões assumidas temporariamente, ex: por um EC2).
- **Políticas** (JSON) definem permissões — princípio do **menor privilégio**.
- **MFA** (autenticação multifator) e boas práticas para a conta **root**.

## 💰 Modelo de preço
- **Gratuito.**

## ⚠️ Pegadinhas de prova
- Use **roles** para dar permissão a serviços/EC2, não chaves embutidas no código.
- **Não use a conta root** no dia a dia; ative MFA nela.
- IAM é **global** (não por região).
- Configurar IAM é responsabilidade **do cliente** ([[Modelo de Responsabilidade Compartilhada]]).

## 🔗 Relacionados
[[KMS]] · [[Organizations]] · [[Modelo de Responsabilidade Compartilhada]]
