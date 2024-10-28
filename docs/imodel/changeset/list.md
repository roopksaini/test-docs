# itp imodel changeset list

List all changesets for a specific iModel.

## Options

- **`--iModelId`**  
  The ID of the iModel whose changesets you want to list.  
  **Type:** `string` **Required:** Yes

- **`--top`**  
  The maximum number of changesets to return.  
  **Type:** `integer` **Required:** No

- **`--skip`**  
  The number of changesets to skip.  
  **Type:** `integer` **Required:** No

- **`--orderBy`**  
  Order the changesets by their index. Can be `asc` for ascending or `desc` for descending order.  
  **Type:** `string` **Required:** No

- **`--afterIndex`**  
  List changesets after a specific index (exclusive).  
  **Type:** `integer` **Required:** No

- **`--lastIndex`**  
  List changesets up to a specific index (inclusive).  
  **Type:** `integer` **Required:** No

## Examples

```bash
# Example 1: List the first 10 changesets for a specific iModel
itp imodel changeset list --iModelId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --top 10

# Example 2: Skip the first 5 changesets and return the next 10
itp imodel changeset list --iModelId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --skip 5 --top 10

# Example 3: List all changesets after a specific index in ascending order
itp imodel changeset list --iModelId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --afterIndex 100 --orderBy "asc"

# Example 4: List all changesets up to a specific index in descending order
itp imodel changeset list --iModelId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --lastIndex 200 --orderBy "desc"
```

## API Reference

[List Changesets](https://developer.bentley.com/apis/imodels-v2/operations/get-imodel-changesets/)
