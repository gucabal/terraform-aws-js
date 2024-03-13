# Simplificar o Gerenciamento de Infraestrutura com Terraform na AWS

## Configurações Iniciais

- Instalar o Terraform:
    - [Download do Terraform](https://www.terraform.io/downloads.html)

- Criar Conta na AWS
    - [Inscrever-se na AWS](https://portal.aws.amazon.com/billing/signup)

- Criar um Usuário no AWS IAM
    - [Configurar IAM](https://docs.aws.amazon.com/rekognition/latest/dg/setting-up.html)

## Desenvolvimento da Aplicação

### Passos Iniciais

- Clonar o Repositório
- Criar um Bucket no Amazon S3
- Configurar Variáveis
    - Substituir `{aws_account_id}` pelo ID da sua conta AWS
    - Substituir `{table_name}` pelo nome da sua tabela do DynamoDB
    - Substituir `{s3_bucket_name}` pelo nome do seu bucket S3 criado anteriormente

- Compactar as Funções Lambda em um Arquivo .zip
- Fazer Upload das Funções Compactadas para o Bucket S3 Criado

### Comandos no Terraform

- Iniciar o Terraform e Baixar Módulos:
  ```
  terraform init
  ```
- Fazer Deploy da Infraestrutura na AWS:
  ```
  terraform apply -auto-approve
  ```