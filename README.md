<h1 align="center">
    <img alt="GoStack" src="https://rocketseat-cdn.s3-sa-east-1.amazonaws.com/bootcamp-header.png" width="200px" />
</h1>

<h3 align="center">
  API GoBarber
</h3>

<p align="justify">🇧🇷 Software de agendamentos online para serviços de barbearia. O projeto foi feito durante o Bootcamp GoStack 10.0. API criada em Node.JS utilizando Express e Sequelize, com tecnologias como autenticação JWT, MongoDB, Redis e PostgreSQL</p>

<p align="justify">🇺🇸 Software for online appointments to barber services. The project was done on the Bootcamp GoStack 10.0. API made in Node.JS using Express and Sequelize, with tecnologies like JWT authentication, MongoDB, Redi and PostgreSQL.</p>

<h1>🇧🇷 Sobre a API</h1>

## Instalação e execução

1. Faça um clone desse repositório;
2. Entre na pasta rodando `cd GoBarber`;
3. Rode `yarn` para instalar as dependências;
4. Crie um banco de dados no `postgres` com o nome de `gobarber`;
5. Crie um banco de dados no `mongodb` com o nome de `gobarber`;
6. Instancie uma base de dados `redis` (será usado para fila de e-mails);
7. Renomeie o arquivo `.env.example` para `.env`;
8. Coloque as suas credenciais dentro do `.env`;
9. Rode `yarn sequelize db:migrate` para executar as migrations;
10. Rode `yarn dev` para iniciar o servidor.
11. Rode `yarn queue` para iniciar o servidor de filas.

## Funcionalidades

### Usuários
- Criação de contas
- Edição de contas
- Upload de imagem (avatar do usuário)
- Conta cliente e conta profissional

### Login
- Login de clientes e profissionais
- Autenticação

### Agendamento
- Notificação de novos agendamentos
- Listagem de horários disponíveis 
- Listagem de horários agendados
- Cancelamento de agendamento (2 horas de antecedência)

## Rotas

<a href="https://documenter.getpostman.com/view/7792112/SzS2wTHE?version=latest" target="_blank">Documentação Postman<a/>

<h1>🇺🇸 About the API</h1>

## Install and Execute

1. Clone this repository;
2. Run the command `cd GoBarber`;
3. Run the command `yarn` to install dependencies;
4. Create a database in `postgres` with the name `gobarber`;
5. Create a database in `mongodb` with the name `gobarber`;
6. Start a `redis` database (used to e-mail's queue);
7. Rename the file `.env.example` to `.env`;
8. Update `.env` with your credentials;
9. Run the command `yarn sequelize db:migrate` to execute the migrations;
10. Run the comman `yarn dev` to start the server.
11. Run the comman `yarn queue` to start the queues server.

## Features

### Users
- Create account
- Update account
- Upload image (user's avatar)
- Customer account and Professional account

### Login
- Login of customers and professionals
- Authentication

### Appointment
- Notification of new appointments
- List all availlable hours
- List all hours with appointments
- Cancel the appointment (at least 2 hours before)

## Routes

<a href="https://documenter.getpostman.com/view/7792112/SzS2wTHE?version=latest" target="_blank">Postman Documentation<a/>

