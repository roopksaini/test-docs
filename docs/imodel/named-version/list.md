# itp imodel named-version list

List all named versions for a specific iModel.

## Options

- **`--iModelId`**  
  The ID of the iModel whose named versions you want to list.  
  **Type:** `string` **Required:** Yes

- **`--top`**  
  Limit the number of named versions returned.  
  **Type:** `integer` **Required:** No

- **`--skip`**  
  Skip a number of named versions in the result.  
  **Type:** `integer` **Required:** No

- **`--orderBy`**  
  Sort by `changesetIndex` or `createdDateTime`, in `asc` or `desc` order.  
  **Type:** `string` **Required:** No

- **`--search`**  
  Search named versions by name or description.  
  **Type:** `string` **Required:** No

- **`--name`**  
  Filter named versions by exact name.  
  **Type:** `string` **Required:** No

## Examples

```bash
# Example 1: List the first 10 named versions for a specific iModel
itp imodel named-version list --iModelId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --top 10

# Example 2: Skip the first 5 named versions and return the next set
itp imodel named-version list --iModelId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --skip 5 --top 10

# Example 3: Search for named versions containing 'Milestone'
itp imodel named-version list --iModelId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --search "Milestone"

# Example 4: Filter named versions by exact name and sort in descending order by changesetIndex
itp imodel named-version list --iModelId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --name "Version 2.0" --orderBy "changesetIndex desc"
```

## API Reference

[Get Named Versions](https://developer.bentley.com/apis/imodels-v2/operations/get-imodel-named-versions/)
