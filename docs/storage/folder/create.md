# itp storage folder create

Create a new folder in a specified parent folder in iTwin's storage.

## Options

- **`--parentFolderId`**  
  The ID of the parent folder where the new folder will be created.  
  **Type:** `string` **Required:** Yes

- **`--displayName`**  
  The display name of the folder to be created.  
  **Type:** `string` **Required:** Yes

- **`--description`**  
  A description of the folder.  
  **Type:** `string` **Required:** No

## Examples

```bash
# Example 1: Create a folder inside the root folder with a description
# Note: You can retrieve the root folder ID using the 'itp storage root-folder' command.
itp storage folder create --parentFolderId "ROOT_FOLDER_ID_HERE" --displayName "Project Documents" --description "Folder for all project-related documents"

# Example 2: Create a subfolder inside an existing folder
itp storage folder create --parentFolderId "b2c3d4e5-6789-01ab-cdef-2345678901bc" --displayName "Design Files"
```

## API Reference

[Create Folder](https://developer.bentley.com/apis/storage/operations/create-folder/)
