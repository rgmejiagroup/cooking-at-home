---
layout: page
---

# Tutorial: Add a new recipe

This tutorial walks you through adding a recipe using the Cooking-at-Home API.

Expect this tutorial to take about 15 minutes to complete.

## Before you start

Make sure you've completed the [Before you start a tutorial](../before-you-start-a-tutorial.md) topic on the development system you'll use for the tutorial.

## Add a new recipe

Adding a new recipe to the service requires that you use the `POST` method to store the details of the new [`recipe`](../api/recipes.md) resource in the service.

To add a new recipe:

1. Make sure your local service is running, or start it by using this command, if it's not:

    ```shell
    cd <your-github-workspace>/cooking-at-home/docs/api
    json-server -w cooking-at-home-db-source.json
    ```

2. Open the Postman app on your desktop.

3. In the Postman app, create a new request with these values:
    * **METHOD**: POST  
    * **URL**: `{{base_url}}/recipes`  
    * **Headers**:
        * `Content-Type: application/json`
    * **Request body**:

    ```json
    {
      "title": "Spicy Tofu Stir Fry",
      "ingredients": ["Tofu", "Garlic", "Chili oil", "Soy sauce"],
      "steps": "Heat oil, fry garlic, add tofu, pour sauces, simmer.",
      "cook_time": "20 minutes"
    }
    ```

4. Choose **Send** to make the request.

5. If successful, the response body should look similar to this:

    ```json
    {
      "title": "Spicy Tofu Stir Fry",
      "ingredients": ["Tofu", "Garlic", "Chili oil", "Soy sauce"],
      "steps": "Heat oil, fry garlic, add tofu, pour sauces, simmer.",
      "cook_time": "20 minutes",
      "id": 5
    }
    ```

You’re now ready to begin adding recipes to your own cooking journal using the Cooking-at-Home API!
