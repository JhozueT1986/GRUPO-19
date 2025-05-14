# SUS Para Todos - Agendamento de Consultas

## Integrantes do Projeto

- Ivan Souza de Oliveira
- Douglas Luiz Gomes de Farias
- Pedro Viana Guedes
- Josué Teixeira do Carmo
- Rian Januario da Costa Santos
- Francisco Walisson Alves Pereira

## Descrição

Projeto: SUS Para Todos
SUS Para Todos é uma aplicação web desenvolvida com o objetivo de simular de forma simples e prática um sistema de agendamento de serviços de saúde, inspirado no funcionamento do SUS (Sistema Único de Saúde) brasileiro. A proposta é fornecer uma experiência básica e acessível para o usuário realizar o cadastro, login, agendamento e confirmação de consultas ou procedimentos médicos, tudo de maneira digital e integrada em um único sistema web.

O projeto foi construído utilizando tecnologias fundamentais do desenvolvimento web: HTML, CSS e JavaScript para o frontend, e Node.js com o framework Express no backend. A persistência de dados é feita localmente por meio de um arquivo JSON (db.json), eliminando a necessidade de um banco de dados externo. Isso torna o projeto ideal para fins educacionais, protótipos rápidos ou demonstrações de conceito (proof of concept).

A aplicação funciona em quatro etapas principais:

Cadastro de Usuário: O usuário acessa a tela de cadastro e informa apenas seu nome e uma senha. Após preencher os dados, o sistema os armazena no arquivo db.json e já registra o usuário como logado automaticamente, simulando uma sessão ativa.

Login: Na tela de login, o sistema solicita nome e senha, permitindo ao usuário acessar a plataforma caso os dados estejam corretos. Caso contrário, uma mensagem de erro é exibida. Não há uso de CPF ou outros documentos pessoais, o que simplifica a experiência do usuário.

Agendamento de Serviço: Após o login, o usuário pode preencher um formulário com os dados do serviço desejado, como tipo de consulta, unidade de saúde, data e horário. Esses dados são vinculados ao usuário logado e também são salvos no db.json.

Confirmação: Após concluir o agendamento, o sistema exibe uma tela de confirmação com o nome do usuário e os dados do serviço agendado, reforçando a simplicidade e eficácia da aplicação.

Toda a navegação entre as telas é feita por HTML estático, com JavaScript controlando as interações, envio de formulários e chamadas à API. O backend Express expõe rotas simples para cadastro (/api/cadastro), login (/api/login), agendamento (/api/agendamento) e confirmação (/api/confirmacao), todas operando diretamente sobre o arquivo JSON.

Além de ser uma aplicação funcional, o projeto SUS Para Todos tem um forte caráter educacional. Ele ensina, na prática, como construir um sistema completo com autenticação, persistência de dados e comunicação entre frontend e backend, sem a complexidade de frameworks pesados ou bancos de dados robustos. É um ótimo ponto de partida para quem está aprendendo desenvolvimento web e deseja entender a integração entre as camadas de uma aplicação real.

Por sua estrutura clara e propósito social, o projeto também pode ser estendido para fins mais complexos, como inclusão de autenticação segura, banco de dados relacional, múltiplos tipos de usuários e integrações com APIs externas. Como está, porém, ele cumpre bem seu papel como base sólida para aprendizado e evolução.

## Tecnologias utilizadas

- **HTML5, CSS3 e JavaScript**: Para estrutura, estilização e interatividade.
- **Framework**: Nenhum framework frontend foi utilizado neste projeto.
- **Backend**: Node.js com Express.js
- **Banco de Dados**: Arquivo local `db.json` (simulação de banco de dados)

## Como executar o projeto

### 1. Requisitos

- Node.js instalado

### 2. Instalar dependências

```bash
npm install
```

### 3. Executar o backend

```bash
npm start
```

O servidor estará disponível em `http://localhost:3000`

### 4. Acessar a aplicação

Abra `http://localhost:3000` no navegador.

---

## Funcionalidades

- Cadastro e login de usuários
- Agendamento de consultas com escolha de especialidade, data e hora
- Visualização de comprovante de agendamento
