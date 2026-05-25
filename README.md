# Minha Primeira Stack com AWS CloudFormation

Este repositório contém a prática do desafio da DIO: **Implementando sua Primeira Stack com AWS CloudFormation**.

## O que foi feito

* Criação de uma pilha simples usando AWS CloudFormation
* Provisionei uma instância EC2 automaticamente via template YAML
* Usei o console da AWS para testar o template e acompanhar a criação dos recursos

## O que aprendi

* O que é infraestrutura como código (IaC)
* Como funciona o AWS CloudFormation
* Como escrever um modelo básico em YAML
* A diferença entre Stack, Template e Recursos
* Automatizar a criação de recursos na AWS evita erros e economiza tempo

## Como testar este modelo

1. Acesse sua conta AWS
2. Vá até o serviço CloudFormation
3. Clique em **Criar Pilha**
4. Faça upload do arquivo `template.yaml`
5. Prossiga com as etapas e crie a Stack
6. Acompanhe o progresso até a finalização

## template.yaml

Este é um exemplo simples de template para criar uma instância EC2 na AWS:

```yaml
AWSTemplateFormatVersion: '2010-09-09'
Description: Minha primeira Stack AWS CloudFormation - Instância EC2 simples

Resources:
  MinhaInstanciaEC2:
    Type: AWS::EC2::Instance
    Properties:
      ImageId: ami-0c55b159cbfafe1f0
      InstanceType: t2.micro
```


