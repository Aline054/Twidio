# TwiDIO API

#### API desenvolvida para o projeto TwiDIO

### Arquitetura

#### 📂Controllers
> Aplica validações necessárias na requisição.
#### 📂Services
> Aplica regras de negócios antes de enviar ao repositório.
#### 📂Repositories
> Salva os dados no banco de dados.
#### 📂Entities
> Gerencia a estrutura das entidades da aplicação.
#### 📂Database
> Cria as conexões necessárias com o banco de dados.

#### 📂__mocks __
> Armazena os dados e mocks utilizados nos testes unitários.
#### 📂tests
> Armazena as switch de testes de integração.



### Este projeto usa
- Node
- Typescript
- Jest
- SQLite
- TypeORM

### Como rodar o projeto

1 - Clone o repositório

2 - Instale todas as dependências

---
    yarn install
---

4 - Acesse a rota principal

<http://localhost:5000/v1/>

### Testando o projeto

#### Testes unitários

---
    yarn test:unit
---

#### Testes de integração

1 - Rode a aplicação em modo de desenvolvimento

---
    yarn run dev
---

1 - Rode os testes de integração no repositório /tests

---
    yarn test:integration
---

### endpoints

**_GET_** /posts

Retorna todos os posts criados no banco de dados

##### Exemplo



**_POST_** /posts (em desenvolvimento)

Cria um novo post no banco de dados. Todos os campos são obrigatórios

##### Exemplo

---
    body {
        author: 'author@email.com',
        content: 'Tuite de exemplo'
    }
---
