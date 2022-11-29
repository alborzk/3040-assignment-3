# Restaurants in Manitoba API

## Description

## Endpoints
- **GET /restaurants** - List all different restaurants in Manitoba
	- Parameters:
		- City (String): The city/town in Manitoba you want to get restaurants from. Optional.
		- Food (String): The type of food keyword(s) you want the restaurants to serve. Optional.
		- Budget (Integer): The maximum cost (in dollars) you are willing to pay for a menu item. Optional.

## Resources

## Example

### Sample request:
```bash
curl -X GET "https://api.restaurants-in-manitoba.org/restaurants?city=winnipeg&food=pizza&budget=30"
```

### Sample response:
```js
[
    {
        name: "Pizza Pizza",
        address: "1740 Pembina Hwy, Winnipeg MB, R3G2G2",
        longitude: 49.827102454465766,
        latitude: -97.15157672949387,
        minPrice: 4.99,
        maxPrice: 47.99
    },
    {
        name: "Pembina's Pizza Joint",
        address: "1743B Pembina Hwy, Winnipeg MB, R3T2G6",
        longitude: 49.826576445541185,
        latitude: -97.15380832742377,
        minPrice: 2.99,
        maxPrice: 19.99
    },
    ...
]
```

### Response definitions
| Response item | Description | Data type |
|-|-|-|
| name | The name of the restaurant. | String |
| address | The human readable address of the restaurant. | String |
| longitude | The longitude coordinate of the restaurant. | Decimal |
| latitude | The latitude coordinate of the restaurant. | Decimal |
| minPrice | The price of the cheapest menu item at the restaurant. | Decimal |
| maxPrice | The price of the most expensive menu item at the restaurant. | Decimal |
