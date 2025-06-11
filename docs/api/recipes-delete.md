## Delete a Recipe

### Goal
Allow users to delete one of their own recipes from the system.

### Prerequisites
- The user must be authenticated.
- The recipe must exist and belong to the user.

### Endpoint
```http
DELETE /recipes/{recipeId}
```

### Success Response
```json
{
  "id": 45,
  "message": "Recipe deleted."
}
```

### Error Handling
- 404 if recipe not found or unauthorized
- 403 if user attempts to delete a recipe not owned by them

---

### Tip
These operations can be combined with a UI modal or confirmation prompt to ensure safe edits and deletions.
