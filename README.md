<h1 align="center">
    <img alt="GoStack" src="https://rocketseat-cdn.s3-sa-east-1.amazonaws.com/bootcamp-header.png" width="200px" />
</h1>

<h3 align="center">
  API GoBarber
</h3>

<p align="justify">Software de agendamentos online para serviços de barbearia. O projeto foi feito durante o Bootcamp GoStack 10.0. API criada em Node.JS utilizando Express e Sequelize, com tecnologias como autenticação JWT, MongoDB, Redis e PostgreSQL</p>

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

Postman: `https://documenter.getpostman.com/view/7792112/SzS2wTHE?version=latest`

