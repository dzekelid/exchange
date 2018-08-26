{
  "info": {
    "name": "Stripe Get Exchange Rates Currency",
    "_postman_id": "7cb49d42-3ac2-489e-9a3f-dfb1ad2b33bf",
    "description": "Retrieves the exchange rates from the given currency to every supported currency.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "exchange",
      "item": [
        {
          "id": "7368cfec-8f7c-4dcc-9c97-da9600a349e8",
          "name": "getExchangeRatesCurrency",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "exchange_rates/:currency"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "currency",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the exchange rates from the given currency to every supported currency"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59ba84e6-975f-41df-a95a-a1a588c8734b"
            }
          ]
        }
      ]
    }
  ]
}