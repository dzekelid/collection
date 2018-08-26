---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/custom_collections.json:
    post:
      summary: Create a new custom collection
      description: Create a new custom collection.
      operationId: postAdminCustomCollections.json
      x-api-path-slug: admincustom-collections-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Custom
      - Collection
  /admin/smart_collections/401912846.json:
    get:
      summary: Get a single collection
      description: Get a single collection.
      operationId: getAdminSmartCollections401912846.json
      x-api-path-slug: adminsmart-collections401912846-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Collection
    put:
      summary: Update a single collection
      description: Update a single collection.
      operationId: putAdminSmartCollections401912846.json
      x-api-path-slug: adminsmart-collections401912846-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Collection
  /admin/custom_collections/246409795.json:
    put:
      summary: update a custom collection
      description: Update a custom collection.
      operationId: putAdminCustomCollections246409795.json
      x-api-path-slug: admincustom-collections246409795-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Update
      - Custom
      - Collection
    delete:
      summary: delete a custom collection
      description: Delete a custom collection.
      operationId: deleteAdminCustomCollections246409795.json
      x-api-path-slug: admincustom-collections246409795-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Delete
      - Custom
      - Collection
  /admin/smart_collections.json:
    get:
      summary: Get all collection
      description: Get all collection.
      operationId: getAdminSmartCollections.json
      x-api-path-slug: adminsmart-collections-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Collection
    post:
      summary: Create a new collection
      description: Create a new collection.
      operationId: postAdminSmartCollections.json
      x-api-path-slug: adminsmart-collections-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Collection
  /admin/collects/921728736.json:
    delete:
      summary: Remove a product from a collection
      description: Remove a product from a collection.
      operationId: deleteAdminCollects921728736.json
      x-api-path-slug: admincollects921728736-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Product
      - From
      - Collection
  /admin/smart_collections/408154574.json:
    delete:
      summary: Delete a single collection
      description: Delete a single collection.
      operationId: deleteAdminSmartCollections408154574.json
      x-api-path-slug: adminsmart-collections408154574-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Collection
  //admin/collects.json:
    post:
      summary: Add a product to a collection
      description: Add a product to a collection.
      operationId: postAdminCollects.json
      x-api-path-slug: admincollects-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - To
      - Collection
---