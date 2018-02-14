# assignment2
wwmdd4999 assignment 2 (recipe db using serverless w/ dynamodb)
melissa chiam

tested in postman.

endpoints:
  POST (add an item)- https://u0j077fkqi.execute-api.us-east-1.amazonaws.com/test/functions
  GET (retrieve list of items from db)- https://u0j077fkqi.execute-api.us-east-1.amazonaws.com/test/functions
  GET (retrieve specific item using key)- https://u0j077fkqi.execute-api.us-east-1.amazonaws.com/test/functions/{recipeId}
  PUT (update specific item using key)- https://u0j077fkqi.execute-api.us-east-1.amazonaws.com/test/functions/{recipeId}
  DELETE (delete a specific item using key)- https://u0j077fkqi.execute-api.us-east-1.amazonaws.com/test/recipe/{recipeId}

instructions:

table:
recipeId (automatic)
recipeDesc (string) - "desc"
recipeIngr (string) = "ingr"
recipeName (string) - "name"

to add an entry, supply data as following example:
```
{

	"name": "recipe3",
 
	"ingr": "lemon juice",
 
	"desc": "squeeze really hard"

}
```
to update or delete an entry, you can get the primary key by first retrieving the list of items, then copy the key into the endpoint.
