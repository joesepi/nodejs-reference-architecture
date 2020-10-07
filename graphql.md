# GraphQL Development

Our teams have extensive knowledge in developing GraphQL solutions.

## Building GraphQL API in from scratch

When building GraphQL API from scratch we recomend using reference implementation which was 
proven to be the most performant and have continous support from community.

### GraphQL Server

Recomending using GraphQL-Express for serving content. 

https://graphql.org/graphql-js/running-an-express-graphql-server

For building GraphQL schema we recomend using GraphQL-Tools:
https://github.com/ardatan/graphql-tools

Developers can use top level database query languages. 
We recomend using Knex(http://knexjs.org/) for performing queries from GraphQL to relational databases.

If your GraphQL model have relationships please consider batching some of the requests by using 
DataLoader: https://github.com/graphql/dataloader

### GraphQL Client

For GraphQL client we recomend URQL (https://formidable.com/open-source/urql/) that can work with React and any other JS based library. 
When using bundler we strongly recomend to compile your graphql queries using GraphQL-Tag.

## Typescript support

If you use typescript in your project we recomend GraphQL-Code-Generator to generate typings for both client and server:

https://graphql-code-generator.com

## Out of the box GraphQL API with CRUD handling

Graphback (https://graphback.dev) can be used to minimize the amount of boilerplate when building GraphQL API.
Graphback is basing on https://graphqlcrud.org specification to deliver out of the box GraphQL API on top of 
popular databases like MongoDB and Postgress.

Graphback can:
- Provide you number of getting started templates
- Mock your backend based on schema (using GraphQL-Serve)
- Build GraphQL resolvers that will fetch data automatically from
- Generate client side queries and fragments for client side minimizing amount of boilerplate
- Providing production ready subscriptions for your model.
- Provide authentication, authorization for your GraphQL API
- Enable datasynchronization (with https://offix.dev used on the client)