# itp access-control member user add

Add one or more user members to an iTwin.

## Options

- **`--iTwinId`**  
  The ID of the iTwin to which the users will be added.  
  **Type:** `string` **Required:** Yes

- **`--members`**  
  A list of members to add, each with an email and a list of role IDs.  
  **Type:** `array` **Required:** Yes

## Examples

```bash
# Example: Add multiple users to an iTwin with role IDs
itp access-control member user add --iTwinId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --members '[
  {"email": "john.johnson@example.com", "roleIds": ["5abbfcef-0eab-472a-b5f5-5c5a43df34b1", "83ee0d80-dea3-495a-b6c0-7bb102ebbcc3"]},
  {"email": "maria.miller@example.com", "roleIds": ["5abbfcef-0eab-472a-b5f5-5c5a43df34b1"]}
]'
```

## API Reference

[Add iTwin User Members](https://developer.bentley.com/apis/access-control-v2/operations/add-itwin-user-members/)
