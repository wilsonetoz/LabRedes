# LabRedes
Este projeto busca demonstrar o uso prático de VLANs e firewalls em ambiente real de nuvem, quanto pelo valor educacional, ao oferecer um laboratório reprodutível para estudantes e profissionais que desejam aprender e aplicar boas práticas em segurança de redes.

# Laboratório de Infraestrutura de Rede Segura na AWS com VLANs e Firewall

## Descrição do Projeto

Este projeto tem como objetivo demonstrar a criação de uma infraestrutura de rede segura e segmentada na nuvem AWS, utilizando subnets como VLANs simuladas e firewalls (Security Groups e NACLs) para o controle de tráfego entre setores.

O laboratório é reprodutível e serve como ferramenta educacional prática para estudantes e profissionais de redes e segurança da informação.

## Arquitetura do Laboratório

A arquitetura do laboratório simula uma instituição de ensino com cinco setores:

| VLAN  | Setor           | Subnet              | Descrição                                  |
|--------|----------------|---------------------|--------------------------------------------|
| VLAN 1 | Administrativo | 172.31.10.0/24      | Direção, RH, Secretaria, Financeiro       |
| VLAN 2 | Acadêmico 1    | 172.31.20.0/24      | Professores, Coordenação                   |
| VLAN 3 | Acadêmico 2    | 172.31.30.0/24      | Alunos, Laboratórios, Pesquisadores       |
| VLAN 4 | TI             | 172.31.40.0/24      | Servidores e Administração de Rede        |
| VLAN 5 | Visitantes     | 172.31.50.0/24      | Rede Wi-Fi pública com acesso à Internet  |

## Recursos Criados

- **VPC Personalizada** (CIDR: 172.31.0.0/16)
- **Subnets privadas e públicas (VLANs simuladas)**
- **Internet Gateway e NAT Gateway**
- **Tabelas de Roteamento**
- **Instâncias EC2:**
    - DNS Server
    - Web Server
    - Servidor de Arquivos
    - Banco de Dados
    - Bastion Host (Acesso SSH)
- **Firewall:**
    - Security Groups (Instância)
    - Network ACLs (Subnet)

## Requisitos

- Conta AWS (Free Tier ou superior)
- Terraform instalado (versão recomendada: >=1.3)
- Chave SSH para acesso via Bastion Host
- Git instalado

## Como Reproduzir o Laboratório

### 1. Clone o repositório:

```bash
git clone https://github.com/seuusuario/laboratorio-vlan-firewall-aws.git
cd laboratorio-vlan-firewall-aws
```
### 2. Configure suas variáveis de ambiente:

copie todo o conteudo do AWS CLI:

<img width="283" height="180" alt="image" src="https://github.com/user-attachments/assets/71889cca-972b-44e6-9890-1b2a6e200ba7" />

cole em .aws/credentials

 ```bash
nano ~/.aws/credentials
```
