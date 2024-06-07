# Agência de Viagens Belo Destino

- Este projeto consiste em criar uma API para uma Agência de Viagens com apenas três tabelas.

### As tabelas possuem os seguintes dados:

- Destinos: id, cidade, valor, data
- Hoteis: id, nome, valor, avaliacao, email, site
- Pontos Turisticos: nome, endereco, telefone, valor

### Consumindo a API

- Criar um Front-End para consumir e enviar dados para esta API.

## Stack utilizada

### ORM- Prisma

- **ORM (Object Relationchip Management)** Gerenciamento de Objeto Relacional

- **PRISMA** - Framework de ORM

- **MVC** - Padrão de projeto 

- **prisma.io** - Documentação 

- **VSCode** - IDE

- **Insomnia** - Testes unitários

- **MYSQL - Mariadb** - Banco de Dados Relacional

- **HTML**

- **CSS**

- **JavaScript**

## Backend

### Iniciando o projeto utilizando Prisma

- Criar uma pasta para o projeto

- Abrir com VSCode

- Instale essas dependências:

- Abrir terminal ( CTRL + " ) no cmd ou bash e instalar o framework globalmente

```bash
npm i -g prisma
```

```bash
npm install cors express dotenv
```

- Para rodar o nodemon

```bash
npm install nodemon
```

- Instalar as dependências do prisma - ver a documentação - database relacional mysql - troca para javascript e instale a dependência. 

```bash
npn install prisma --save-dev
```

- Iniciar o projeto com o ORM Prisma e a biblioteca do SGBD, uso no caso o MySQL - MariaDB

```bash
npx prisma init --datasource-provider mysql
```

-  Editar o arquivo com a variável de ambiente com a string de conexão com o Banco de dados, quando o App for implantado esta string será alterada com as configuraçõe do servidor SGBD.
.env

```bash
DATABASE_URL="mysql://root:@localhost:3306/nome_banco_de_dados"
```

- Criar os Modelos de tabelas e relacionamentos no arquivo ./prisma/shema.prisma 
schema.prisma.

- Executar a primeira migração. Inicialize o XAMPP, start em MYSQL e APACHE e abra o PhpMyAdmin. Para as tabelas aparecerem digite o comando:

```bash
npx prisma migrate dev --name init
```
- Instale essas extensões no VSC ( Prisma e Prisma Inside ).

- Instale as dependências do Prisma Client.

```bash
npm install @prisma/client
```

- Editar os controllers criando os CRUDS. 

- Criar as rotas
./src/routes.js

- Editar o server
server.js

- Executar a API

```bash
nodemon
```

- Testar com Insomnia, Postman ou outra ferramenta de teste unitário de sua preferência.

## Front-end

### Como executar o projeto

- Para conhecer todas as páginas do projeto, clique em index.html e abra com o Live Server do VSCode para navegar por todo o site.

- O projeto esta em fase de melhorias conforme o avanço nos estudos.

## Print das Telas

- Tela 1

![tela 1](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/741a9153-d669-4832-85be-a3e2dbad851c)

- Tela 2

![tela 2](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/3974e2c7-496a-4b73-a2b9-659949dc881a)

- Tela 3

![destinos](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/7430e08a-a2ab-4618-997e-ecdff9d3eaab)

- Tela 3 - Botão Adicionar Destino

![pagina destinos](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/c7600b6b-1bce-48af-b405-006561e630ae)

- Modal Adicionar Destino

![modal adicionar destino](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/bebf57c9-952d-4d81-931c-5767f842dcb1)

- Modal Editar Destino

![modal editar destino](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/d51f7e03-3e72-4998-957d-2ef4bb96cfaa)

- Tela 4

![hoteis](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/1abb7d9a-a7d7-4cb2-b714-3acd53485b7f)

- Tela 5

![pontos](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/628585eb-85e7-4b6b-84bf-86d4c2665b34)

- Tela 6

![tela 6](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/87a3ea73-8660-47e2-807f-5d74ede4dd81)

## Autores

- [@octokatherine](https://www.github.com/Carla-coder)

## Instituição de Ensino

- Escola Senai unidade Jaguariúna - Curso Técnico em Desenvolvimento de Sistemas FullStack  Segundo Semestre (2024)

- Professor responsável pelo Projeto: Wellington Fabio https://github.com/wellifabio
