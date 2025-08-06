# 🧪 Laboratório Prático em Nuvem com VLANs e Firewall na AWS

Este projeto tem como objetivo fornecer um **laboratório reprodutível para fins educacionais**, simulando a segmentação lógica de uma rede institucional utilizando recursos da AWS, como VPCs, subnets, Security Groups, NACLs e automação com Terraform.

---

## 📌 Objetivos

- Demonstrar a aplicação de VLANs simuladas com subnets na AWS.
- Aplicar regras de firewall com Security Groups e NACLs.
- Automatizar a infraestrutura utilizando Terraform.
- Proporcionar um ambiente de aprendizagem prática sobre segurança e segmentação de redes.

---

## 🧱 Infraestrutura Simulada

A arquitetura do laboratório representa a rede de uma instituição de ensino com cinco blocos (VLANs):

- **VLAN 1 - Administrativo**
- **VLAN 2 - Acadêmico 1**
- **VLAN 3 - Acadêmico 2**
- **VLAN 4 - Tecnologia da Informação (TI)**
- **VLAN 5 - Visitantes**

Recursos implementados:

- Subnets isoladas
- Internet Gateway e NAT Gateway
- Tabelas de rotas
- Instâncias EC2 (DNS, Web, Arquivos, Banco de Dados, Bastion Host)
- Regras de segurança com SGs e NACLs

---

## ⚙️ Tecnologias Utilizadas

- [Amazon Web Services (AWS)](https://aws.amazon.com/)
- [Terraform](https://developer.hashicorp.com/terraform)
- Linux (Ubuntu Server ou Amazon Linux 2)
- Git e GitHub

---

## 🚀 Como Usar

### Pré-requisitos

- Conta ativa na AWS
- Terraform instalado
- Chave SSH gerada para acesso remoto às instâncias

### Passos

1. **Clone este repositório**:

```bash
git clone https://github.com/wilsonetoz/LabRedes.git
cd LabRedes
```

3. **Executar Terraform**:

```bash
terraform init
terraform plan
terraform apply
```
Acessar o Bastion Host:

Utilize a chave SSH para se conectar e realizar a configuração manual dos servidores internos.

---
📚 Documentação

---
🎓 Público-Alvo

Este projeto foi desenvolvido para estudantes de redes, professores e profissionais que desejam aprender na prática os conceitos de:
*Segmentação de redes*

*Segurança em nuvem*

*Automação de infraestrutura*

---
🤝 **Contribuições**

Contribuições são bem-vindas!

1- Abra uma issue

2- Faça um fork do repositório

3-Crie um branch para sua feature ou correção

4- Envie um pull request
