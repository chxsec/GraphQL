# Check if GraphQL suggestions are enabled
## Exmaples using deliberately misspelled queries
```
{"query":"{ __typ(name: \"Query\") { name } }"}
```

```
{"query":"{ usrs { id } }"}
```

#### Exmaple of response if suggestions are enabled
```
{
  "errors": [
    {
      "message": "Cannot query field \"usrs\" on type \"Query\". Did you mean \"users\"?"
    }
  ]
}
```
