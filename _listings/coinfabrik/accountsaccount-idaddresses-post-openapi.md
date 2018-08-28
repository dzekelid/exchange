---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 0
info:
  title: CoinFabrik Create address
  description: "Creates a new address for an account. As all the arguments are optinal,
    it\u2019s possible just to do a empty POST which will create a new address. This
    is handy if you need to create new receive addresses for an account on-demand.\nAddresses
    can be created for all account types. With fiat accounts, funds will be received
    with Instant Exchange."
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}/addresses:
    post:
      summary: Create address
      description: "Creates a new address for an account. As all the arguments are
        optinal, it\u2019s possible just to do a empty POST which will create a new
        address. This is handy if you need to create new receive addresses for an
        account on-demand.\nAddresses can be created for all account types. With fiat
        accounts, funds will be received with Instant Exchange."
      operationId: creates-a-new-address-for-an-account-as-all-the-arguments-are-optinal-its-possible-just-to-do-a-empt
      x-api-path-slug: accountsaccount-idaddresses-post
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: body
        name: address_properties
        description: Properties to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Address
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