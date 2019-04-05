
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

```graphql

mutation {
  book(date: "2019-03-11T00:00:00Z", role: Speaker, title: "Hey buddy") {
    date
    agenda {
      role
      title
      duration
      member{
        name
        mobile
        email
        id
      }
    }
  }
}

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

// Query for meetings
{
  meetings {
    id
    agenda {
      role
    }
    date
  }
}
```
