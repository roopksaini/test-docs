# itp access-control group delete

Delete an existing group from an iTwin.

## Options

- **`--iTwinId`**  
  The ID of the iTwin where the group exists.  
  **Type:** `string` **Required:** Yes

- **`--groupId`**  
  The ID of the group to be deleted.  
  **Type:** `string` **Required:** Yes

## Examples

```bash
itp access-control group delete --iTwinId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --groupId "bf4d8b36-25d7-4b72-b38b-12c1f0325f42"
```

## API Reference

[Delete iTwin Group](https://developer.bentley.com/apis/access-control-v2/operations/delete-itwin-group/)
