---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph List Table Collection
  description: List TableCollection Retrieve a list of table objects.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /workbook/names:
    get:
      summary: List Named Item Collection
      description: List NamedItemCollection Retrieve a list of nameditem objects.
      operationId: ListNamedItemCollection
      x-api-path-slug: workbooknames-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Named
      - Item
      - Collection
  /workbook/names(&lt;name&gt;)/range/format/borders:
    get:
      summary: List Range Border Collection
      description: List RangeBorderCollection Retrieve a list of rangeborder objects.
      operationId: ListRangeBorderCollection
      x-api-path-slug: workbooknamesltnamegtrangeformatborders-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Range
      - Border
      - Collection
  /workbook/worksheets(&lt;id|name&gt;)/range(&lt;address&gt;)/format/borders:
    get:
      summary: List Range Border Collection
      description: List RangeBorderCollection Retrieve a list of rangeborder objects.
      operationId: ListRangeBorderCollection
      x-api-path-slug: workbookworksheetsltidnamegtrangeltaddressgtformatborders-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Range
      - Border
      - Collection
  /workbook/tables(&lt;id|name&gt;)/columns(&lt;id|name&gt;)/range/format/borders:
    get:
      summary: List Range Border Collection
      description: List RangeBorderCollection Retrieve a list of rangeborder objects.
      operationId: ListRangeBorderCollection
      x-api-path-slug: workbooktablesltidnamegtcolumnsltidnamegtrangeformatborders-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Range
      - Border
      - Collection
  /workbook/names(&lt;name&gt;)/range/format/borders/ItemAt:
    post:
      summary: Range Border Collection Item At
      description: 'RangeBorderCollection: ItemAt Gets a border object using its index'
      operationId: RangeBorderCollection:ItemAt
      x-api-path-slug: workbooknamesltnamegtrangeformatbordersitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Range
      - Border
      - Collection
      - Item
      - At
  /workbook/worksheets(&lt;id|name&gt;)/range(&lt;address&gt;)/format/borders/ItemAt:
    post:
      summary: Range Border Collection Item At
      description: 'RangeBorderCollection: ItemAt Gets a border object using its index'
      operationId: RangeBorderCollection:ItemAt
      x-api-path-slug: workbookworksheetsltidnamegtrangeltaddressgtformatbordersitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Range
      - Border
      - Collection
      - Item
      - At
  /workbook/tables(&lt;id|name&gt;)/columns(&lt;id|name&gt;)/range/format/borders/ItemAt:
    post:
      summary: Range Border Collection Item At
      description: 'RangeBorderCollection: ItemAt Gets a border object using its index'
      operationId: RangeBorderCollection:ItemAt
      x-api-path-slug: workbooktablesltidnamegtcolumnsltidnamegtrangeformatbordersitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Range
      - Border
      - Collection
      - Item
      - At
  /workbook/tables:
    get:
      summary: List Table Collection
      description: List TableCollection Retrieve a list of table objects.
      operationId: ListTableCollection
      x-api-path-slug: workbooktables-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Table
      - Collection
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