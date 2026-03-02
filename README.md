# Lab – Introdução ao Amazon EC2

## 📌 Visão Geral
Este projeto documenta a execução do laboratório **Introdução ao Amazon EC2**, cujo objetivo é apresentar os conceitos fundamentais do serviço **Amazon Elastic Compute Cloud (EC2)**, incluindo criação, configuração, acesso e gerenciamento básico de instâncias.

O laboratório fornece uma base sólida para compreender como servidores virtuais funcionam na nuvem da **(AWS)**, abordando aspectos essenciais de **compute, rede e segurança**.

---

## 🎯 Objetivos do Laboratório
Ao final deste laboratório, fui capaz de:

- Compreender o conceito de **instância EC2**
- Criar e iniciar uma instância EC2
- Selecionar uma **AMI (Amazon Machine Image)**
- Escolher o tipo de instância adequado
- Configurar **Key Pair** para acesso seguro
- Configurar **Security Group** para controle de tráfego
- Acessar a instância via **SSH**
- Encerrar a instância corretamente

---

## 🛠️ Serviços e Tecnologias Utilizadas
- **Amazon EC2**
- **Amazon Machine Image (AMI)**
- **Security Groups**
- **Key Pair (SSH)**
- **Amazon VPC (default)**
- **Amazon Linux 2**
- **AWS Management Console**

---

## 🧱 Arquitetura Básica
A arquitetura do laboratório é composta por:

- Uma instância **EC2**
- Subnet pública da VPC padrão
- IP público atribuído automaticamente
- Security Group atuando como firewall
- Acesso remoto via SSH

📸 Evidência:  
`screenshots/architecture-overview.png`

---

## ⚙️ Etapas Executadas

### 1️⃣ Acesso ao AWS Management Console
- Início do laboratório em ambiente educacional
- Acesso ao console AWS fornecido pelo lab
- Uso da região padrão do laboratório

📸 Evidência:  
`screenshots/01-aws-console.png`

---

### 2️⃣ Criação da Instância EC2
Configurações principais da instância:

- Nome da instância: `EC2-Lab-Instance`
- AMI: **Amazon Linux 2**
- Tipo da instância: `t2.micro`
- VPC: padrão (default)
- Subnet: pública
- IP público: habilitado

📸 Evidência:  
`screenshots/02-ec2-instance-creation.png`

---

### 3️⃣ Configuração do Key Pair
- Utilização de **Key Pair** fornecida pelo laboratório
- Chave usada para autenticação segura via SSH
- Download e armazenamento seguro da chave

📸 Evidência:  
`screenshots/03-key-pair.png`

---

### 4️⃣ Configuração do Security Group
O Security Group foi configurado como firewall da instância:

**Regras de entrada (Inbound Rules):**
- SSH (porta 22) – acesso remoto
- Origem: Anywhere IPv4 (apenas para fins de laboratório)

📸 Evidência:  
`screenshots/04-security-group.png`

---

### 5️⃣ Inicialização da Instância
- Instância lançada com sucesso
- Verificação de status:
  - State: Running
  - Status checks: 2/2 passed

📸 Evidência:  
`screenshots/05-ec2-running.png`

---

### 6️⃣ Acesso à Instância via SSH
A instância foi acessada remotamente utilizando SSH:

- Usuário padrão: `ec2-user`
- Autenticação via Key Pair
- Conexão bem-sucedida ao sistema operacional

📸 Evidência:  
`screenshots/06-ssh-access.png`

---

### 7️⃣ Verificação do Ambiente
Após o acesso, foram realizados testes básicos:

- Verificação do sistema operacional
- Confirmação do hostname da instância
- Teste de conectividade

📸 Evidência:  
`screenshots/07-ec2-terminal.png`

---

### 8️⃣ Encerramento da Instância
- Instância encerrada corretamente
- Liberação de recursos do laboratório
- Evita custos e mantém boas práticas

📸 Evidência:  
`screenshots/08-ec2-terminated.png`

---

## 🔐 Boas Práticas de Segurança Aplicadas
- Uso de autenticação por **Key Pair**
- Controle de acesso via **Security Group**
- Encerramento de recursos após uso
- Princípio do menor privilégio (contexto do lab)

---

## 📚 Principais Conceitos Aprendidos
- O que é o Amazon EC2
- Diferença entre AMI e tipo de instância
- Função do Security Group como firewall
- Importância do Key Pair para acesso seguro
- Ciclo de vida de uma instância EC2
- Acesso remoto via SSH
- Gerenciamento básico de recursos na AWS

---

## 🚀 Próximos Passos
- Instalar um servidor web (Apache ou Nginx)
- Automatizar configurações com User Data
- Criar instâncias em VPC customizada
- Associar EC2 a IAM Roles
- Monitorar instâncias com CloudWatch
- Criar imagens personalizadas (AMI)

---

## 📝 Observação
Este laboratório foi executado em um **ambiente educacional (AWS Training / Vocareum)**, com recursos temporários e limites controlados.

---

## 👩‍💻 Autora
**Hortência França**  
Profissional em transição para **Cloud Computing e Cibersegurança**, com foco em **Cloud Júnior / Analista de SOC Júnior**.
