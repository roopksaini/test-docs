# itp access-control group info

Retrieve details about a specific group in an iTwin.

## Options

- **`--iTwinId`**  
  The ID of the iTwin where the group exists.  
  **Type:** `string` **Required:** Yes

- **`--groupId`**  
  The ID of the group to retrieve information about.  
  **Type:** `string` **Required:** Yes

## Examples

```bash
itp access-control group info --iTwinId "ad0ba809-9241-48ad-9eb0-c8038c1a1d51" --groupId "bf4d8b36-25d7-4b72-b38b-12c1f0325f42"
```

## API Reference

[Get iTwin Group Info](https://developer.bentley.com/apis/access-control-v2/operations/get-itwin-group/)
