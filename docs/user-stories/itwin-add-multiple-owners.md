# Add multiple owners to an iTwin

## Scenario

As a user, I want to add multiple owners to an iTwin so that different team members can have full access to manage the project.

## Steps

1. **Create an iTwin**: Start by creating a new iTwin (if one doesn't already exist).
2. **Add owner 1**: Assign the first owner to the iTwin.
3. **Add owner 2**: Assign the second owner to the iTwin.
4. **Add owner 3**: Assign the third owner to the iTwin.

## Commands Used

- `itp itwin create`  
  Creates a new iTwin.

- `itp access-control member owner add`  
  Adds an owner to the iTwin.

## Example

Step 1: Create an iTwin
```bash
itp itwin create --displayName "New Infrastructure Project" --description "iTwin for managing infrastructure project"
```

Step 2: Add owner 1 to the iTwin
```bash
itp access-control member owner add --iTwinId "your-itwin-id" --email "owner1@example.com"
```

Step 3: Add owner 2 to the iTwin
```bash
itp access-control member owner add --iTwinId "your-itwin-id" --email "owner2@example.com"
```

Step 4: Add owner 3 to the iTwin
```bash
itp access-control member owner add --iTwinId "your-itwin-id" --email "owner3@example.com"
```

## Expected Outcome

After following these steps, you will have successfully created an iTwin and added three owners to it, giving them full administrative access to the project.

## Next Steps

- **Manage Owners**: You can update the list of owners later by adding or removing users as needed.
