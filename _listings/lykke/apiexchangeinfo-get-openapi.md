---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API Exchangeinfo
  version: 1.0.0
  description: Get api exchangeinfo.
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