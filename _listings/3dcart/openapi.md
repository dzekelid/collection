---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 1
info:
  title: _3dCartWebAPI
  version: 1.0.0
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Categories/{categoryid}/Options:
    put:
      summary: Updates a collection of options from a specific Category
      description: Updates a collection of options from a specific category.
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-put
      parameters:
      - in: path
        name: categoryid
        description: CategoryID
      - in: body
        name: options
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Options
      - From
      - Specific
      - Category
  /3dCartWebAPI/v1/CustomerGroups:
    put:
      summary: This method updates a collection of customer groups in the database.
        No URL parameters should be included.
      description: This method updates a collection of customer groups in the database.
        no url parameters should be included..
      operationId: CustomerGroups_Update
      x-api-path-slug: 3dcartwebapiv1customergroups-put
      parameters:
      - in: body
        name: customergroups
        description: A Json or XML object containing the customer group
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Updates
      - Collection
      - Of
      - Customer
      - Groups
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
  /3dCartWebAPI/v1/Orders/{orderid}/Items:
    put:
      summary: Updates a collection of items from a specific Order
      description: Updates a collection of items from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-put
      parameters:
      - in: body
        name: items
        description: A Json or XML object containing the new items
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Items
      - From
      - Specific
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Questions:
    put:
      summary: Updates a collection of questions from a specific Order
      description: Updates a collection of questions from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: questions
        description: A Json or XML object containing the new questions
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Questions
      - From
      - Specific
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Shipments:
    put:
      summary: Updates a collection of shipments from a specific Order
      description: Updates a collection of shipments from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidshipments-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: shipments
        description: A Json or XML object containing the new shipments
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Shipments
      - From
      - Specific
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Transactions:
    put:
      summary: Updates a collection of transactions from a specific Order
      description: Updates a collection of transactions from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transactions
        description: A Json or XML object containing the new transactions
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Transactions
      - From
      - Specific
      - Order
  /3dCartWebAPI/v1/Products/{catalogid}/AdvancedOptions:
    put:
      summary: Updates a collection of advanced options from a specific Product
      description: Updates a collection of advanced options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidadvancedoptions-put
      parameters:
      - in: body
        name: advancedoptions
        description: A Json or XML object containing the new advanced options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Advanced
      - Options
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Discount:
    put:
      summary: Updates a collection of discounts from a specific Product
      description: Updates a collection of discounts from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogiddiscount-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: discounts
        description: A Json or XML object containing the new discount
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Discounts
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/EProducts:
    put:
      summary: Updates a collection of eproducts from a specific Product
      description: Updates a collection of eproducts from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogideproducts-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: eproducts
        description: A Json or XML object containing the new features
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Eproducts
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Features:
    put:
      summary: Updates a collection of features from a specific Product
      description: Updates a collection of features from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidfeatures-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: features
        description: A Json or XML object containing the new features
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Features
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Images:
    put:
      summary: Updates a collection of images from a specific Product
      description: Updates a collection of images from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidimages-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: images
        description: A Json or XML object containing the new images
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Images
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Options:
    put:
      summary: Updates a collection of options from a specific Product
      description: Updates a collection of options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidoptions-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: options
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Options
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Related:
    put:
      summary: Updates a collection of related products from a specific Product
      description: Updates a collection of related products from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidrelated-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: relatedproducts
        description: A Json or XML object containing the new related products
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Related
      - Products
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Serials:
    put:
      summary: Updates a collection of serials from a specific Product
      description: Updates a collection of serials from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidserials-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: serials
        description: A Json or XML object containing the new serials
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Serials
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/UpSelling:
    put:
      summary: Updates a collection of upselling items from a specific Product
      description: Updates a collection of upselling items from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidupselling-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: upsellingitems
        description: A Json or XML object containing the new upselling items
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Upselling
      - Items
      - From
      - Specific
      - Product
---