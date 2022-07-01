Quais problemas GraphQL resolve?

- Overfetching
  - http://Localhost : 3000/users
  - DB (USuários, endereços)
- Underfetching
  - http://localhost : 3800/users
  - DB (usuários)
  - http://localhost: 3000/addresses

Dificuldades :

- Cache
- Erros

```gql
query {
  users {
    id
    name
    github
    addresses {
      city
      state
      country
    }
  }
}
```
