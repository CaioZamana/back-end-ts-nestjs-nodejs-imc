<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Projeto de Exemplo usando Node.js e NestJS

Este é um projeto de exemplo que utiliza Node.js e NestJS para criar um serviço simples de cálculo de IMC (Índice de Massa Corporal).

## Pré-requisitos

Certifique-se de ter Node.js instalado em sua máquina. Você pode baixá-lo em [nodejs.org](https://nodejs.org/en).

## Instalação

### 1. Instale o NestJS CLI globalmente executando o seguinte comando:
npm install -g @nestjs/cli

### 2. Se você estiver usando o PowerShell no Windows, é necessário configurar a política de execução para permitir scripts não assinados. Execute o seguinte comando no PowerShell como administrador:
Set-ExecutionPolicy RemoteSigned

## Configuração do Projeto

### 1. Crie um novo projeto NestJS executando o seguinte comando:
nest new back-end-node-nest

### 2. Navegue até o diretório do projeto:
cd project-name

## Executando o Serviço

### Para iniciar o serviço, execute o seguinte comando:
npm start

### Após a inicialização, você pode acessar o serviço através do seguinte URL:
http://localhost:3000/

# Este serviço fornece dois endpoints:

## 1. GET /:weight/:height

###    Este endpoint calcula o IMC (Índice de Massa Corporal) com base no peso e altura fornecidos como parâmetros na URL.

###   Exemplo:
    GET http://localhost:3000/91/1.93

Isso retornará uma mensagem indicando o IMC calculado.

## 2. GET /

### Este endpoint retorna uma mensagem de saudação.

###   Exemplo:
    GET http://localhost:3000

Isso retornará uma mensagem "Hello World!".

## O projeto consiste em dois principais componentes:

- AppController: Responsável por manipular as requisições HTTP e chamar os serviços apropriados.

- AppService: Contém a lógica de negócios para o cálculo do IMC e a mensagem de saudação.