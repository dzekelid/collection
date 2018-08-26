---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Worksheet Collection Add
  description: 'WorksheetCollection: add Adds a new worksheet to the workbook. The
    worksheet will be added at the end of existing worksheets. If you wish to activate
    the newly added worksheet, call ".activate() on it.'
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
  /workbook/worksheets(&lt;id|name&gt;)/tables:
    get:
      summary: List Table Collection
      description: List TableCollection Retrieve a list of table objects.
      operationId: ListTableCollection
      x-api-path-slug: workbookworksheetsltidnamegttables-get
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
  /workbook/tables/add:
    post:
      summary: Table Collection Add
      description: 'TableCollection: add Create a new table. The range source address
        determines the worksheet under which the table will be added. If the table
        cannot be added (e.g., because the address is invalid, or the table would
        overlap with another table), an error will be thrown.'
      operationId: TableCollection:Add
      x-api-path-slug: workbooktablesadd-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Collection
  /workbook/worksheets(&lt;id|name&gt;)/tables/add:
    post:
      summary: Table Collection Add
      description: 'TableCollection: add Create a new table. The range source address
        determines the worksheet under which the table will be added. If the table
        cannot be added (e.g., because the address is invalid, or the table would
        overlap with another table), an error will be thrown.'
      operationId: TableCollection:Add
      x-api-path-slug: workbookworksheetsltidnamegttablesadd-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Collection
  /workbook/tables(&lt;id|name&gt;)/columns/add:
    post:
      summary: Table Column Collection Add
      description: 'TableColumnCollection: add Adds a new column to the table.'
      operationId: TableColumnCollection:Add
      x-api-path-slug: workbooktablesltidnamegtcolumnsadd-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Column
      - Collection
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/columns/add:
    post:
      summary: Table Column Collection Add
      description: 'TableColumnCollection: add Adds a new column to the table.'
      operationId: TableColumnCollection:Add
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtcolumnsadd-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Column
      - Collection
  /workbook/tables(&lt;id|name&gt;)/columns/ItemAt:
    post:
      summary: Table Column Collection Item At
      description: 'TableColumnCollection: ItemAt Gets a column based on its position
        in the collection.'
      operationId: TableColumnCollection:ItemAt
      x-api-path-slug: workbooktablesltidnamegtcolumnsitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Column
      - Collection
      - Item
      - At
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/columns/ItemAt:
    post:
      summary: Table Column Collection Item At
      description: 'TableColumnCollection: ItemAt Gets a column based on its position
        in the collection.'
      operationId: TableColumnCollection:ItemAt
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtcolumnsitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Column
      - Collection
      - Item
      - At
  /workbook/tables(&lt;id|name&gt;)/rows/add:
    post:
      summary: Table Row Collection Add
      description: 'TableRowCollection: add Adds a new row to the table.'
      operationId: TableRowCollection:Add
      x-api-path-slug: workbooktablesltidnamegtrowsadd-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Row
      - Collection
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/rows/add:
    post:
      summary: Table Row Collection Add
      description: 'TableRowCollection: add Adds a new row to the table.'
      operationId: TableRowCollection:Add
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtrowsadd-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Row
      - Collection
  /workbook/tables(&lt;id|name&gt;)/rows/ItemAt:
    post:
      summary: Table Row Collection Item At
      description: 'TableRowCollection: ItemAt Gets a row based on its position in
        the collection.'
      operationId: TableRowCollection:ItemAt
      x-api-path-slug: workbooktablesltidnamegtrowsitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Row
      - Collection
      - Item
      - At
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/rows/ItemAt:
    post:
      summary: Table Row Collection Item At
      description: 'TableRowCollection: ItemAt Gets a row based on its position in
        the collection.'
      operationId: TableRowCollection:ItemAt
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtrowsitemat-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Table
      - Row
      - Collection
      - Item
      - At
  /workbook/worksheets/:
    post:
      summary: Worksheet Collection Add
      description: 'WorksheetCollection: add Adds a new worksheet to the workbook.
        The worksheet will be added at the end of existing worksheets. If you wish
        to activate the newly added worksheet, call ".activate() on it.'
      operationId: WorksheetCollection:Add
      x-api-path-slug: workbookworksheets-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - Worksheet
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