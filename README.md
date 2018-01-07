# Error

> Schema must be an instance of GraphQLSchema. Also ensure that there are not multiple versions of GraphQL installed in your node_modules directory.


## Reproduction

```sh
graphcool deploy
yarn
yarn start
```

```graphql
# works
query a {
  feed {
    id
  }
}
```

```graphql
subscription c {
  publications {
    node {
      id
    }
  }
}
```

results in Error

> Schema must be an instance of GraphQLSchema. Also ensure that there are not multiple versions of GraphQL installed in your node_modules directory.
