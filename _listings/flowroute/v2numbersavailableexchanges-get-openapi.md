---
swagger: "2.0"
x-collection-name: Flowroute
x-complete: 0
info:
  title: FlowRoute API List Available Exchange Codes
  description: Returns a list of all Central Office (exchange) codes containing purchasable
    phone numbers.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/numbers/available/exchanges:
    get:
      summary: List Available Exchange Codes
      description: Returns a list of all Central Office (exchange) codes containing
        purchasable phone numbers.
      operationId: returns-a-list-of-all-central-office-exchange-codes-containing-purchasable-phone-numbers
      x-api-path-slug: v2numbersavailableexchanges-get
      parameters:
      - in: query
        name: areacode
        description: Restricts the results to the specified area code
      - in: query
        name: limit
        description: Limits the number of items to retrieve
      - in: query
        name: max_setup_cost
        description: Restricts the results to exchanges that include at least one
          telephone number with a setup fee below or equal to the specified max_setup_cost
      - in: query
        name: offset
        description: Offsets the list of phone numbers by your specified value
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - List
      - Available
      - Exchange
      - Codes
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---