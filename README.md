# CRUD API RESTful com Laravel e React JS

## 📌 Sobre o Projeto
Este repositório contém um projeto de estudo prático focado na construção de uma **API RESTful** do zero. O projeto consiste em um sistema **CRUD** (Create, Read, Update, Delete) de usuários, onde o **Back-End** foi desenvolvido utilizando o framework **Laravel (PHP)**.

A API foi projetada para interagir e ser consumida por uma aplicação **Front-End** desenvolvida em **React JS**.

> **Aviso:** A parte desenvolvida por mim, seguindo os passos do canal Eduteka, como forma de estudo e prática, abrange **exclusivamente o Back-End**. A interface Front-End foi entregue pronta pelo canal EDUTEKA para que a integração pudesse ser testada.

## 🔗 Links e Referências
* **Vídeo de Estudo (EDUTEKA):** [Como Criar uma API RESTful do Zero com Laravel e Consumir com React JS](https://www.youtube.com/watch?v=jLGKI_zMftU)
* **Repositório do Front-End (Fornecido):** [eduteka-course-apirest-frontend](https://github.com/edutekabr/eduteka-course-apirest-frontend)

## 🛠️ Tecnologias Utilizadas (Back-End)
* **PHP**
* **Laravel** (Controllers, Requests, API Resources, Eloquent ORM)
* **SQLite** (Banco de Dados)

## 📁 Estrutura do Projeto

Abaixo está a organização principal das pastas e arquivos do Back-End desenvolvido em Laravel. A arquitetura foi pensada para manter a organização, segurança e padronização das respostas da API.

```text
📦 CRUD-APIRESTFul
 ┣ 📂 app
 ┃ ┣ 📂 Http
 ┃ ┃ ┣ 📂 Controllers
 ┃ ┃ ┃ ┗ 📜 UserController.php      # Controla a lógica principal do CRUD (Index, Store, Show, Update, Destroy)
 ┃ ┃ ┣ 📂 Requests
 ┃ ┃ ┃ ┣ 📜 StoreUserRequest.php    # Regras de segurança e validação para criar um usuário
 ┃ ┃ ┃ ┗ 📜 UpdateUserRequest.php   # Regras de segurança e validação para atualizar um usuário
 ┃ ┃ ┗ 📂 Resources
 ┃ ┃   ┣ 📜 UserResource.php        # Formata a estrutura JSON de resposta para um único usuário
 ┃ ┃   ┗ 📜 UserCollection.php      # Formata a estrutura JSON para listagens (com suporte a paginação)
 ┃ ┗ 📂 Models
 ┃   ┗ 📜 User.php                  # Modelo de representação da tabela de usuários no banco de dados
 ┣ 📂 database
 ┃ ┣ 📂 factories
 ┃ ┃ ┗ 📜 UserFactory.php           # Fábrica para geração de dados falsos (para testes)
 ┃ ┣ 📂 migrations
 ┃ ┃ ┗ 📜 ...create_users_table.php # Estrutura de criação da tabela de usuários no banco
 ┃ ┗ 📂 seeders
 ┃   ┗ 📜 DatabaseSeeder.php        # Popula automaticamente o banco de dados via terminal
 ┣ 📂 routes
 ┃ ┗ 📜 api.php                     # Arquivo onde todas as rotas da API RESTful foram registradas
 ┣ 📜 .env.example                  # Variáveis de ambiente (Configuração do banco, portas, etc.)
 ┗ 📜 README.md                     # Documentação do projeto
