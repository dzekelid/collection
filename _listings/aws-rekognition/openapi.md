---
swagger: "2.0"
x-collection-name: AWS Rekognition
x-complete: 1
info:
  title: AWS Rekognition API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateCollection:
    get:
      summary: Create Collection
      description: Creates a collection in an AWS Region.
      operationId: createCollection
      x-api-path-slug: actioncreatecollection-get
      parameters:
      - in: query
        name: CollectionId
        description: ID for the collection that you are creating
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Collections
  /?Action=DeleteCollection:
    get:
      summary: Delete Collection
      description: Deletes the specified collection.
      operationId: deleteCollection
      x-api-path-slug: actiondeletecollection-get
      parameters:
      - in: query
        name: CollectionId
        description: ID of the collection to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Collections
  /?Action=ListCollections:
    get:
      summary: List Collections
      description: Returns list of collection IDs in your account.
      operationId: listCollections
      x-api-path-slug: actionlistcollections-get
      parameters:
      - in: query
        name: MaxResults
        description: Maximum number of collection IDs to return
        type: string
      - in: query
        name: NextToken
        description: Pagination token from the previous response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Collections
---