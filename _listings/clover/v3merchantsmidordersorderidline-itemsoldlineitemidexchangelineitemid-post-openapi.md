---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Create or exchange a line item
  version: 1.0.0
  description: Create or exchange a line item.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/orders/{orderId}/line_items/{oldLineItemId}/exchange/{lineItemId}:
    post:
      summary: Create or exchange a line item
      description: Create or exchange a line item.
      operationId: SetOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: oldLineItemId
        description: Old Line Item Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - OldLineItemId
      - Exchange
      - LineItemId
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