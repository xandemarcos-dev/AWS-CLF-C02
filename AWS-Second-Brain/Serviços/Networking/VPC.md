---
servico: VPC
dominio: Networking
tags: [aws, networking, clf-c02]
nivel: clf-c02
---

# Amazon VPC (Virtual Private Cloud)

## Em uma frase
> Sua rede privada e isolada dentro da AWS, onde você lança os recursos.

## O que é / pra que serve
Rede virtual logicamente isolada onde ficam [[EC2]], [[RDS]] etc. Você define faixas
de IP, sub-redes, rotas e regras de segurança. É a base de networking da sua conta.

## Quando usar (e quando NÃO usar)
- ✅ Sempre que precisa isolar/controlar a rede dos seus recursos.
- ❌ — (é fundamento; quase tudo roda dentro de uma VPC).

## Conceitos-chave
- **Sub-redes públicas vs privadas** (com/sem acesso à internet).
- **Security Groups:** firewall **da instância** (stateful).
- **Network ACLs (NACL):** firewall **da sub-rede** (stateless).
- **Internet Gateway** (acesso à internet) e **NAT Gateway** (saída para sub-rede privada).

## 💰 Modelo de preço
- A VPC em si é gratuita; alguns componentes custam (NAT Gateway, VPN, tráfego entre AZs/regiões).

## ⚠️ Pegadinhas de prova
- **Security Group** = nível da instância (stateful); **NACL** = nível da sub-rede (stateless).
- Sub-rede **pública** tem rota para Internet Gateway; **privada** não.
- VPC é isolada por conta/região.

## 🔗 Relacionados
[[EC2]] · [[Route 53]] · [[ELB]] · [[Regiões, AZs e Edge Locations]]
