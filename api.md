
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

