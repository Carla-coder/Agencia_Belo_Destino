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

![destinos1](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/9dbf697f-e68e-4b6e-a8fe-9663dbce63d3)

- Modal Adicionar Destino

![modal adicionar destino](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/72ebce3e-28af-47fb-84c8-05bfeb7c041f)

- Modal Editar Destino

![modal editar destino](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/d51f7e03-3e72-4998-957d-2ef4bb96cfaa)

- Tela 4

![hoteis1](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/3c8b8e6d-4608-49f5-b509-f67ace8561fb)

- Modal Adicionar Hotel

![adicionar hotel](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/71ccdacc-9770-4302-91e3-0cfbd8939afd)

- Modal Editar Hotel

![editar hotel](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/1df0b740-b791-430d-8034-0a97a2ed4db1)

- Tela 5

![pontos1](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/b91c7e0f-96fd-48e6-b838-5acde8cb441a)

- Modal Adicionar Ponto

![adicionar ponto](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/e4c1d45c-3691-4e9e-992d-1aa5018886df)

- Modal Editar Ponto

![editar ponto](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/0fc00ff2-f60a-4304-b8b2-369ff027be19)

- Tela 6

![tela 6](https://github.com/Carla-coder/Agencia_Belo_Destino/assets/128012862/87a3ea73-8660-47e2-807f-5d74ede4dd81)

## Autores

- [@octokatherine](https://www.github.com/Carla-coder)

## Instituição de Ensino

- Escola Senai unidade Jaguariúna - Curso Técnico em Desenvolvimento de Sistemas FullStack  Segundo Semestre (2024)

- Professor responsável pelo Projeto: Wellington Fabio https://github.com/wellifabio
