---
swagger: "2.0"
info:
  title: Akamai API Add an Element
  description: Add an Element
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /network-list/v1/network_lists/{networkListId}/element:
    put:
      summary: Add an Element
      description: Add an Element
      operationId: networklistv1network-listsnetworklistidelement
      parameters:
      - in: query
        name: networkListId
        description: Unique identifier for the network list, corresponding to the
          unique-id within the data
        type: string
      responses:
        200:
          description: OK
      tags:
      - network
      - list
      - network
      - lists
      - networklist
      - element
definitions: []
x-collection-name: Akamai
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