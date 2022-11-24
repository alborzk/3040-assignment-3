# Restaurants in Manitoba API

### Description

### Endpoints
- List all different restaurants in Manitoba
	- Parameters:
		- City (String): The city/town in Manitoba you want to get restaurants from. Optional.
		- Food (String): The type of food keyword(s) you want the restaurants to serve. Optional.
		- Budget (Int): The maximum cost (in dollars) you are willing to pay for a menu item. Optional.

### Resources

### Examples

- List("Winnipeg", "pizza", 12)
	- Lists restaraunts with pizza under $12.
	- Returns Dominos, Pizza Pizza, etc...
- List()
	- Lists ALL restaruants in the database.
- List("Winnipeg", "burger")
	- Lists all restaurants that have burgers, regardless of price.
	- Returns Tony Romas, McDonalds, Wendys, Red Lobster, etc.
