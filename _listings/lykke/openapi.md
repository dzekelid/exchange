---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/BcnTransactionByExchange/{id}:
    get:
      summary: Get API Bcntransactionbyexchange
      description: Get api bcntransactionbyexchange.
      operationId: ApiBcnTransactionByExchangeByIdGet
      x-api-path-slug: apibcntransactionbyexchangeid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransactionbyexchange
  /api/ExchangeInfo:
    get:
      summary: Get API Exchangeinfo
      description: Get api exchangeinfo.
      operationId: ApiExchangeInfoGet
      x-api-path-slug: apiexchangeinfo-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: exchangeId
      responses:
        200:
          description: OK
      tags:
      - Exchangeinfo
---