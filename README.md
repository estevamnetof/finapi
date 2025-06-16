# Finapi
## Uma API RESTful para simulação de operações bancárias básicas, desenvolvida com Node.js e Express.

### 📋 Funcionalidades 

✅ Criar conta bancária

✅ Consultar extrato

✅ Fazer depósitos

✅ Realizar saques

✅ Atualizar dados da conta

✅ Deletar conta

✅ Consultar saldo

✅ Filtrar extrato por data

### 🚀 Como Executar
Pré-requisitos
Node.js instalado

NPM ou Yarn

### Instalação
## Clone o repositório
git clone https://github.com/estevamnetof/finapi.git

## Acesse a pasta do projeto
cd finapi

## Instale as dependências
npm install
### ou
yarn install
Iniciando a API
npm start
### ou
yarn start
A API estará disponível em: http://localhost:3333

## 📚 Documentação da API
Rotas Disponíveis
Método	Endpoint	Descrição

POST	/account	Cria uma nova conta

GET	/account	Retorna dados da conta

PUT	/account	Atualiza dados da conta

DELETE	/account	Remove uma conta

GET	/statement	Retorna o extrato completo

GET	/statement/date	Retorna extrato por data específica

GET	/balance	Retorna o saldo atual

POST	/deposit	Realiza um depósito

POST	/withdraw	Realiza um saque

## Exemplos de Uso
### Criar conta:

POST /account
Headers: { "Content-Type": "application/json" }

Body: { "cpf": "12345678900", "name": "Fulano da Silva" }

### Consultar saldo:

GET /balance
Headers: { "cpf": "12345678900" }

### Fazer depósito:

POST /deposit

Headers: { "cpf": "12345678900" }

Body: { "description": "Depósito inicial", "amount": 1000 }

## 🛠 Tecnologias Utilizadas
Node.js

Express

UUID (para geração de IDs únicos)

## 📝 Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
