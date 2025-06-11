---
## Update a Recipe

### Goal
Allow users to update details of a saved recipe such as ingredients, steps, or title.

### Prerequisites
- The user must be authenticated.
- The recipe must already exist and belong to the user.

### Endpoint
```http
PATCH /recipes/{recipeId}
```

### Request Body Example
```json
{
  "title": "Spicy Tofu Stir Fry",
  "ingredients": [
    "Tofu", "Garlic", "Chili oil", "Soy sauce"
  ],
  "steps": "Heat oil, fry garlic, add tofu, pour sauces, simmer."
}
```

### Response Example
```json
{
  "id": 45,
  "message": "Recipe updated successfully."
}
```

### Error Handling
- 404 if the recipe is not found or not owned by the user
- 400 if payload is malformed

---
