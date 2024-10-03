# Check for GraphQL
[Return to README](https://github.com/chxsec/GraphQL/blob/main/README.md)
## GraphQL Request
```
query {
          __typename
}
```
## POST Request
```
{"query": "query {\n    __typename\n}"}
```
## POST simplified
```
{"query": "query {__typename}"}
```
## GET Query
```
GET /graphql?query=query%7B__typename%7D
```
