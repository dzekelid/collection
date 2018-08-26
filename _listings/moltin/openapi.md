---
swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/collections/{collectionID}/relationships/collections:
    post:
      summary: Create Collection Relationships
      description: Create collection relationships.
      operationId: V2CollectionsRelationshipsCollectionsByCollectionIDPost
      x-api-path-slug: v2collectionscollectionidrelationshipscollections-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
      - Relationships
  /v2/collections:
    post:
      summary: Create a Collection
      description: Create a collection.
      operationId: V2CollectionsPost
      x-api-path-slug: v2collections-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
  /v2/collections/{collectionID}:
    get:
      summary: Get a Collection
      description: Get a collection.
      operationId: V2CollectionsByCollectionIDGet
      x-api-path-slug: v2collectionscollectionid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      - in: query
        name: filter
      - in: query
        name: include
      - in: query
        name: page[limit]
      - in: query
        name: page[offset]
      - in: query
        name: sort
      responses:
        200:
          description: Successful response
      tags:
      - Collection
    put:
      summary: Update a Collection
      description: Update a collection.
      operationId: V2CollectionsByCollectionIDPut
      x-api-path-slug: v2collectionscollectionid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
    delete:
      summary: Delete a Collection
      description: Delete a collection.
      operationId: V2CollectionsByCollectionIDDelete
      x-api-path-slug: v2collectionscollectionid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
  /v2/collections/{collectionID}/relationships/parent:
    put:
      summary: Update Parent Collection Relationship
      description: Update parent collection relationship.
      operationId: V2CollectionsRelationshipsParentByCollectionIDPut
      x-api-path-slug: v2collectionscollectionidrelationshipsparent-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Collection
      - Relationship
    post:
      summary: Create Parent Collection Relationship
      description: Create parent collection relationship.
      operationId: V2CollectionsRelationshipsParentByCollectionIDPost
      x-api-path-slug: v2collectionscollectionidrelationshipsparent-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Collection
      - Relationship
    delete:
      summary: Delete Parent Collection Relationship
      description: Delete parent collection relationship.
      operationId: V2CollectionsRelationshipsParentByCollectionIDDelete
      x-api-path-slug: v2collectionscollectionidrelationshipsparent-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Collection
      - Relationship
  /v2/collections/tree:
    get:
      summary: Get Collection tree
      description: Get collection tree.
      operationId: V2CollectionsTreeGet
      x-api-path-slug: v2collectionstree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
      - Tree
  /v2/collections/{collectionID}/relationships/children:
    put:
      summary: Update Child Collection Relationship
      description: Update child collection relationship.
      operationId: V2CollectionsRelationshipsChildrenByCollectionIDPut
      x-api-path-slug: v2collectionscollectionidrelationshipschildren-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Collection
      - Relationship
    post:
      summary: Create Child Collection Relationships
      description: Create child collection relationships.
      operationId: V2CollectionsRelationshipsChildrenByCollectionIDPost
      x-api-path-slug: v2collectionscollectionidrelationshipschildren-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Collection
      - Relationships
    delete:
      summary: Delete Child Collection Relationship
      description: Delete child collection relationship.
      operationId: V2CollectionsRelationshipsChildrenByCollectionIDDelete
      x-api-path-slug: v2collectionscollectionidrelationshipschildren-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Collection
      - Relationship
---