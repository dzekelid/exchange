---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Get Reserved Instances Exchange Quote
  version: 1.0.0
  description: Returns details about the values and term of your specified Convertible
    Reserved Instances.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcceptReservedInstancesExchangeQuote:
    get:
      summary: Accept Reserved Instances Exchange Quote
      description: Accepts the Convertible Reserved Instance exchange quote described
        in the GetReservedInstancesExchangeQuote call.
      operationId: acceptreservedinstancesexchangequote
      x-api-path-slug: actionacceptreservedinstancesexchangequote-get
      parameters:
      - in: query
        name: ReservedInstancesListingId
        description: The ID of the Reserved Instance listing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
  /?Action=GetReservedInstancesExchangeQuote:
    get:
      summary: Get Reserved Instances Exchange Quote
      description: Returns details about the values and term of your specified Convertible
        Reserved Instances.
      operationId: getreservedinstancesexchangequote
      x-api-path-slug: actiongetreservedinstancesexchangequote-get
      parameters:
      - in: query
        name: ClientToken
        description: A unique, case-sensitive token you provide to ensure idempotency
          of your modification request
        type: string
      - in: query
        name: ReservedInstancesConfigurationSetItemType.N
        description: The configuration settings for the Reserved Instances to modify
        type: string
      - in: query
        name: ReservedInstancesId.N
        description: The IDs of the Reserved Instances to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
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