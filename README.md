# Projeto: Infraestrutura Básica com Amazon EC2

## Objetivo

Criar uma infraestrutura simples na AWS utilizando uma instância EC2 para hospedar uma aplicação web.

![AWS](https://img.shields.io/badge/AWS-CloudFormation-orange?style=for-the-badge&logo=amazonaws)  
![Bootcamp](https://img.shields.io/badge/DIO-Bootcamp-success?style=for-the-badge)  

## Arquitetura

Usuário
    │
Internet
    │
Internet Gateway
    │
VPC
    │
Subnet Pública
    │
Security Group
    │
Amazon EC2

## Diagrama: 📊

![Diagrama da Infraestrutura](./infraestrutura-basica.drawio.png)

## Serviços Utilizados

**Amazon EC2**
**Amazon VPC**
**Internet Gateway**
**Security Group**
*Amazon EBS**
**Par de Chaves (Key Pair)**

## Componentes Utilizados: 🛠️
- **Usuário (Cliente):** Origem das requisições para a aplicação.  
- **Internet:** Representa a rede pública que conecta os usuários à AWS.  
- **Internet Gateway (IGW):** Permite a comunicação entre a VPC e a Internet.  
- **VPC (Virtual Private Cloud):** Rede isolada dentro da AWS onde os recursos foram provisionados.  
- **Subnet Pública:** Sub-rede dentro da VPC que contém recursos acessíveis pela Internet.  
- **EC2 Instance:** Máquina virtual onde a aplicação pode ser hospedada.  
- **Security Group:** Firewall virtual que controla as regras de entrada e saída da instância EC2.  

## Etapas do Projeto: 🔗
1 . Criar uma **VPC**.

2 . Criar uma **Subnet Pública**.

3 . Configurar o **Internet Gateway**.

4 . Criar um **Security Group** liberando as portas:
**22 (SSH)**
**80 (HTTP)**

5 . Criar uma **instância Amazon EC2**.

6 . Conectar **via SSH**.

7 . Instalar **um servidor web** (Apache ou Nginx).

8 . Testar o **acesso pelo navegador**.

## Fluxo de Comunicação: 🔗
1. O **usuário** acessa a aplicação pela **Internet**.  
2. O tráfego passa pelo **Internet Gateway (IGW)**.  
3. Dentro da **VPC**, a requisição chega até a **Subnet Pública**.  
4. A **EC2** processa a requisição, respeitando as regras definidas no **Security Group**.  

---


Esse é um diagrama **básico**, que pode ser expandido futuramente.

---

## Melhorias Futuras

**Adicionar Load Balancer**.

**Configurar Auto Scaling**.

**Utilizar Amazon RDS**.

**Armazenar arquivos no Amazon S3**.

**Monitorar com Amazon CloudWatch**.

**Automatizar a criação da infraestrutura utilizando AWS**

 **CloudFormation ou Terraform**.
