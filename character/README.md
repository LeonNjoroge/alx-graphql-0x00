# GraphQL Character Query Solutions

This project contains two GraphQL query solutions using the [Rick and Morty GraphQL API](https://rickandmortyapi.com/graphql).

## Solution 1: Fetching a Character by ID

The query uses the `character(id: ID!)` field to retrieve details of a specific character by their ID. For this solution, IDs 1 through 4 were tested. The selected fields include:

- `id`
- `name`
- `status`
- `species`
- `type`
- `gender`

Each query returns a single character object containing those six fields. The solution demonstrates how to format a GraphQL query that accepts a single ID argument and returns a consistent shape of data, even if some fields (like `type`) are empty.

## Solution 2: Fetching a Paginated List of Characters

This query utilizes the `characters(page: Int)` field to retrieve a paginated list of characters. Pages 1 through 4 were queried to verify the pagination mechanism.

From each page’s result, the `results` array was accessed, and the following fields were selected for every character:

- `id`
- `name`
- `status`
- `image`

The solution showcases how to query nested results and iterate through multiple pages to explore the full dataset.