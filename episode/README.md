# GraphQL Episode Query Solution

This project includes a solution query for retrieving information about a specific episode using the `episode(id: ID!)` field from the [Rick and Morty GraphQL API](https://rickandmortyapi.com/graphql).

## Solution: Get a Specific Episode by ID

The query demonstrates how to fetch a single episode by its unique ID. It includes the required fields:

- `id`
- `name`
- `air_date`
- `episode`

The query returns the episode's metadata, allowing the learner to understand how scalar fields are accessed through root-level queries with arguments.

### Example Query (Episode ID: 1)

```graphql
query Episode {
  episode(id: 1) {
    id
    name
    air_date
    episode
  }
}
