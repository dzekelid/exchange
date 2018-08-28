swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 1
info:
  title: Coinbase API
  description: the-coinbase-v2-api
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