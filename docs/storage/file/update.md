# itp storage file update

Update the metadata of a file in an iTwin's storage, such as display name or description.

## Options

- **`--fileId`**  
  The ID of the file to be updated.  
  **Type:** `string` **Required:** Yes

- **`--displayName`**  
  The new display name for the file.  
  **Type:** `string` **Required:** No

- **`--description`**  
  A description for the file.  
  **Type:** `string` **Required:** No

## Examples

```bash
# Example 1: Update file display name
itp storage file update --fileId "bf4d8b36-25d7-4b72-b38b-12c1f0325f42" --displayName "Updated Design File"

# Example 2: Update file description and display name
itp storage file update --fileId "c9f2b8a5-345d-4cfa-b3e5-123456789abc" --displayName "New Model File" --description "Updated model with new specifications"
```

## API Reference

[Update File](https://developer.bentley.com/apis/storage/operations/update-file/)
