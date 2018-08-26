{
  "info": {
    "name": "Stripe Get Exchange Rates",
    "_postman_id": "b7b1f61a-5036-4a48-aebd-ea3e97c464c4",
    "description": "Returns a list of objects that contain the rates at which foreign currencies are converted to one another. Only shows the currencies for which Stripe supports.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "exchange",
      "item": [
        {
          "id": "a614dbe0-4d6b-44a1-8257-64711e601d8f",
          "name": "getExchangeRates",
          "request": {
            "url": "http://api.stripe.com/v1/exchange_rates?ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of objects that contain the rates at which foreign currencies are converted to one another"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ae1d08f-4a83-4e2c-a886-c7e45a3bff09"
            }
          ]
        }
      ]
    }
  ]
}