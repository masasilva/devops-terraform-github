# devops-terraform-jenkins

Este repositório contém exemplos de **scripts** e **pipelines** para integrar **Terraform** e **Jenkins** em um processo de **CI/CD** (Integração Contínua e Entrega Contínua). O objetivo é automatizar a criação de infraestrutura em nuvem (exemplo com AWS), utilizando o **Terraform** e **Jenkins** para realizar o deploy e automação de aplicações.

## Estrutura do Repositório

- **terraform/**: Scripts relacionados ao Terraform, como configuração de recursos, variáveis, outputs e planos de aplicação.
- **jenkins/**: Pipelines e scripts de integração com o Jenkins para executar processos de CI/CD com Terraform.

## Pré-requisitos

Antes de começar, verifique se você possui os seguintes pré-requisitos instalados:

- [Terraform](https://www.terraform.io/downloads) (versão 1.x)
- [Jenkins](https://www.jenkins.io/download/) (versão 2.x)
- Conta na AWS (ou outro provedor de nuvem) configurada no Terraform
- Jenkins com o plugin **Terraform** instalado

## Como Usar

### 1. Configuração do Terraform

#### a. Variáveis
O Terraform utiliza arquivos de variáveis para definir informações como regiões e tipos de instância. Exemplo de configuração:

```hcl
variable "aws_region" {
  description = "A região da AWS onde os recursos serão criados"
  type        = string
  default     = "us-east-1"
}

variable "instance_type" {
  description = "Tipo da instância EC2"
  type        = string
  default     = "t2.micro"
}
