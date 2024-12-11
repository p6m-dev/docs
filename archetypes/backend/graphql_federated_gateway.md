# GraphQL Federated Gateway Archetype

A `GraphQL Federated Gateway` is a component in a distributed GraphQL system that acts as an entry point for clients, enabling them to interact with multiple underlying GraphQL services (also called subgraphs) as if they were a single API. It uses GraphQL Federation, a specification introduced by Apollo, to manage and orchestrate multiple GraphQL schemas.


## Generate
```sh 
archetect
```
`P6M -> Platform -> GraphQL Federated Gateway`

## Configuration
1. Update your `registry.yaml` to replace `default-domain-gateway` with the name of your service.
    1. Update the `routing_url` to match domain gateway's the service name in kubernetes
        1. This is generally `http://{service-name}.{service-name}:8080/graphql`
    2. Update the `automation` section to match your organization and repository name.
    3. Update the `file` to match the name of your subgraph file.
2. [Optional] Enable Auth2.0 JWT authorization
   1. Uncomment the Auth2.0 section in the `config/router.yaml` file
   2. Fill in your Auth2.0 endpoint