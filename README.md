# ignite-desafio04-database-queries
Desafio 01 - Database Queries

Objetivo
Realizar consultas no banco de dados com o TypeORM de três formas:

- ORM
- Query Builder
- Raw Query
 

Vamos criar o conteiner:

docker run --name ignite-challenge-database-queries -e POSTGRES_DB=queries_challenge -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres

Quando o desafio estiver finalizado, você pode parar o container com o comando docker stop ignite-challenge-database-queries para que não fique consumindo recursos desnecessários da sua máquina. 
`docker stop ignite-challenge-database-queries`

E caso você tenha parado o container ou reiniciou sua máquina mas ainda precisa do container rodando, é possível iniciá-lo novamente com o comando docker start ignite-challenge-database-queries.
`docker start ignite-challenge-database-queries`

## Requisitos:

### UsersRepository:

 - findUserWithGamesById
 - findAllUsersOrderedByFirstName
 - findUserByFullName

#### GamesRepository

 - findByTitleContaining
 - countAllGames
 - findUsersByGameId

## Específicação dos testes

## OBS Teste do model:
- ```Para rodar os teste: yarn test```

### UsersRepository

 - Should be able to find user with games list by user's ID
 - Should be able to list users ordered by first name
 - Should be able to find user by full name

### GamesRepository

 - Should be able find a game by entire or partial given title
 - Should be able to get the total count of games
 - Should be able to list users who have given game id


img


## Instalação

```
# Clone este repositório
$ git clone

# Instale as dependências
$ yarn ou yarn install

# Para rodar os teste: 
$ yarn test
```
