swagger: "2.0"
x-collection-name: Flowroute
x-complete: 1
info:
  title: Flowroute APIs
  description: the-flowroute-apis-are-organized-around-rest--our-apis-have-resourceoriented-urls-support-http-verbs-and-respond-with-http-status-codes--all-api-requests-and-responses-including-errors-will-be-represented-as-json-objects--you-can-use-the-flowroute-apis-to-manage-your-flowroute-phone-numbers-including-setting-primary-and-failover-routes-for-inbound-calls-and-sending-text-messages-sms-and-mms-using-longcode-or-tollfree-numbers-in-your-account-
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