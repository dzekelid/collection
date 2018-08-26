---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/properties/groups/{groupId}/properties:
    post:
      summary: Mass attach propertyId and groupId collection into the pivot table.
      description: Mass attach propertyid and groupid collection into the pivot table..
      operationId: postRestPropertiesGroupsGroupProperties
      x-api-path-slug: restpropertiesgroupsgroupidproperties-post
      parameters:
      - in: path
        name: groupId
      responses:
        200:
          description: OK
      tags:
      - Mass
      - Attach
      - PropertyId
      - GroupId
      - Collection
      - Into
      - Pivot
      - Table
---