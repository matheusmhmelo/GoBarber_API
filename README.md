<h1 align="center">
    <img alt="GoStack" src="https://rocketseat-cdn.s3-sa-east-1.amazonaws.com/bootcamp-header.png" width="200px" />
</h1>

<h3 align="center">
  API GoBarber
</h3>

<p align="justify">Software de agendamentos online para serviços de barbearia. O projeto foi feito durante o Bootcamp GoStack 10.0 e ainda será melhorado.
  Entre algumas funcionalidades da API estão: cadastro de usuários, cadastro de profissionais, login e autenticação com JWT, upload de arquivos,
  notificações por e-mail, filas de gerenciamento de e-mail utilizando Redis, tratamento de exceções entre outras.</p>

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

## Rotas

### POST

`/users` (name, email, password) - Criação de conta
<br/>
`/session` (email, password) - Login
<br/>
`/files` (file, auth::userId) - Upload logo
<br/>
`/appointments` (provider_id, date, auth::userId) - Agendamento

### GET

`/providers` (auth::userId) - Lista profissionais
<br/>
`/providers/:providerId/available` (auth::userId) - Lista horários disponíveis
<br/>
`/appointments` (auth::userId) - Lista todos agendamento
<br/>
`/schedule` (auth::userId) - Lista agendamentos do profissional
<br/>
`/notifications` (auth::userId) - Lista todas as notificações

### PUT

`/users` (name, email, oldPassword, password, confirmPassword, avatar_id, auth::userId) - Atualizar usuário
<br/>
`/notifications/:id` (auth::userId) - Marca notificação como lida

### DELETE

`/appointments/:id` (auth::userId) - Cancela agendamento

<br/>
<p>:warning: (auth::userId)* Autenticação necessária para acessar a rota. Token referente ao usuário (obtido em <b>/session</b>).</p>
<br/>
<p>:warning: <b>API ainda em desenvolvimento</b> :warning:</p>
