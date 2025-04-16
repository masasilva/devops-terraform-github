# devops-terraform-github

Este repositório contém exemplos de **pipelines CI/CD** com **Jenkins** e automações com **Terraform**. O objetivo é demonstrar como integrar **Jenkins** com **Terraform** para provisionamento de infraestrutura na nuvem, além de automações em diversas plataformas, incluindo o uso de **GitHub** para gerenciamento de código.

## Descrição

Este repositório serve como uma demonstração de **CI/CD** utilizando **Jenkins** e **Terraform**, com a capacidade de integrar e automatizar processos a partir de um repositório no **GitHub**. O exemplo inicial mostrará como criar uma infraestrutura na **Azure** utilizando o Terraform com Jenkins, com código armazenado no GitHub.

## Estrutura do Repositório

- **terraform/**: Scripts para provisionamento de infraestrutura, como VMs, redes, etc., utilizando o Terraform.
- **jenkins/**: Scripts de pipeline Jenkins para integração com Terraform e automações.
- **github/**: Arquivos de configuração e integração com o GitHub.

## Pré-requisitos

- [Terraform](https://www.terraform.io/downloads) (versão 1.x)
- [Jenkins](https://www.jenkins.io/download/) (versão 2.x)
- Conta no **GitHub** e repositório configurado.
- Conta na **Azure** (ou outro provedor de nuvem) e credenciais configuradas.
- **Jenkins** configurado com credenciais para acessar o **GitHub** e a **Azure**.

## Como Usar

### 1. Configuração do Terraform

- Navegue até o diretório **terraform/**.
- Edite as variáveis no arquivo `variables.tf` conforme suas necessidades (exemplo: credenciais, nome da VM, etc.).
- Execute os comandos Terraform para provisionar a infraestrutura:

```bash
terraform init
terraform validate
terraform plan
terraform apply
