
CI Server
https://dt-be.herokuapp.com/

```graphql
# Query for testing
{
  hello
}
```


```graphql
# Register a user
mutation {
  register(person: {name: "owen", password: "pwd"})
}
```

```graphql
# Then login and get user ID
{
  login(user: "owen", password: "pwd")
}
```

mutation {
  book(person: "5c85eaa75ee116b982774e61", date: "20190909", role: TMD, title: "hehe") {
   id
    agenda {
      role {
        name
        member {
          name
        }
      }
      duration
      title
    }
    date
  }
}
