# devops-terraform-github

Este repositório contém exemplos de **CI/CD** e automações com **GitHub** e **Terraform**. O objetivo é demonstrar como integrar **GitHub Actions** com **Terraform** para provisionamento de infraestrutura na nuvem, automações e automação de deploys.

## Descrição

Este repositório é uma demonstração de **CI/CD** utilizando **GitHub Actions** e **Terraform**, com a capacidade de automatizar o provisionamento de infraestrutura utilizando o Terraform a partir de um repositório no **GitHub**. O exemplo inicial demonstra como criar infraestrutura na **Azure** utilizando o Terraform através de ações do GitHub.

## Estrutura do Repositório

- **terraform/**: Scripts para provisionamento de infraestrutura, como VMs, redes, etc., utilizando o Terraform.
- **github-actions/**: Arquivos de configuração para **GitHub Actions** para automação e integração com Terraform.
- **README.md**: Documentação explicando como usar e configurar os scripts.

## Pré-requisitos

- [Terraform](https://www.terraform.io/downloads) (versão 1.x)
- Conta no **GitHub** e repositório configurado.
- Conta na **Azure** (ou outro provedor de nuvem) com credenciais configuradas.
- **GitHub Actions** habilitado no repositório.

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
