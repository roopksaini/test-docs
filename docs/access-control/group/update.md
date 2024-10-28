# itp access-control group update

Update the details of an existing group in an iTwin.

## Options

- **`--iTwinId`**  
  The ID of the iTwin where the group exists.  
  **Type:** `string` **Required:** Yes

- **`--groupId`**  
  The ID of the group to be updated.  
  **Type:** `string` **Required:** Yes

- **`--name`**  
  The updated name of the group.  
  **Type:** `string` **Required:** No

- **`--description`**  
  The updated description of the group.  
  **Type:** `string` **Required:** No

- **`--members`**  
  A list of members (emails) to be assigned to the group.  
  **Type:** `array of strings` **Required:** No

- **`--imsGroups`**  
  A list of IMS Groups to be linked to the group.  
  **Type:** `array of strings` **Required:** No

## Examples

```bash
# Example 1: Update group name and description
itp access-control group update --iTwinId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --groupId "bf4d8b36-25d7-4b72-b38b-12c1f0325f42" --name "Updated Engineering Team" --description "Updated description"

# Example 2: Update group members and IMS groups
itp access-control group update --iTwinId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --groupId "bf4d8b36-25d7-4b72-b38b-12c1f0325f42" --members '["john.doe@example.com", "jane.doe@example.com"]' --imsGroups '["Sample IMS Group"]'
```

## API Reference

[Update iTwin Group](https://developer.bentley.com/apis/access-control-v2/operations/update-itwin-group/)
