---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Customer APIs Retrieves the confirmed production
    option
  description: Retrieves the production option confirmed as the finalized production
    requirements, and the initial pricing for it.
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborationRooms/{collaborationRoomId}/productionData:
    get:
      summary: Retrieves the production data
      description: Retrieves the production data in a collaboration room, including
        the currency, all the production options, and the initial pricings provided
        by the supplier.
      operationId: retrieves-the-production-data-in-a-collaboration-room-including-the-currency-all-the-production-opti
      x-api-path-slug: collaborationroomscollaborationroomidproductiondata-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Production
      - Data
    post:
      summary: Creates a production option
      description: "Creates a new production option, providing the pricing information
        in the meantime.  \nThe login user must be a collaboration lead from the additive
        manufacturing supplier."
      operationId: creates-a-new-production-option-providing-the-pricing-information-in-the-meantime--the-login-user-mu
      x-api-path-slug: collaborationroomscollaborationroomidproductiondata-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: body
        name: ProductionDataCreateRequest
        description: A request about creating a production option
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/productionData/basic:
    post:
      summary: Creates a production option without pricing
      description: "Creates a new production option without an initial pricing.  \nThis
        endpoint is used by users from the additive manufactuirng supplier that're
        not collaboration leads."
      operationId: creates-a-new-production-option-without-an-initial-pricing--this-endpoint-is-used-by-users-from-the-
      x-api-path-slug: collaborationroomscollaborationroomidproductiondatabasic-post
      parameters:
      - in: body
        name: AdditionalProductionDataBasicCreateRequest
        description: A request about creating a production option without pricing
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Production
      - Option
      - Without
      - Pricing
  /collaborationRooms/{collaborationRoomId}/productionData/original/requirement:
    put:
      summary: Updates the customer's production option
      description: "Updates the customer's production option.   \nThe login user must
        be from the customer."
      operationId: updates-the-customers-production-option---the-login-user-must-be-from-the-customer
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataoriginalrequirement-put
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: body
        name: ProductionDataRequirementRequest
        description: A request about a production option
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Customers
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/productionData/{productionDataId}:
    put:
      summary: Updates a supplier's production option
      description: "Updates a production option proposed by the additive manufacturing
        supplier as well as the initial pricing for this option.  \nThe login user
        must be a collaboration lead from the additive manufacturing supplier."
      operationId: updates-a-production-option-proposed-by-the-additive-manufacturing-supplier-as-well-as-the-initial-p
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataproductiondataid-put
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: productionDataId
        description: The ID of a production option
      - in: body
        name: ProductionDataUpdateRequest
        description: A request about updating a production option
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Suppliers
      - Production
      - Option
    delete:
      summary: Deletes a supplier's production option
      description: "Deletes a production option proposed by the additive manufacturing
        supplier. The initial pricing is deleted along with it.  \nThe login user
        must be from the additive manufacturing supplier."
      operationId: deletes-a-production-option-proposed-by-the-additive-manufacturing-supplier-the-initial-pricing-is-d
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataproductiondataid-delete
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: productionDataId
        description: The ID of a production option
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Suppliers
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/productionData/{productionDataId}/basic:
    put:
      summary: Updates a supplier's production option
      description: "Updates a production option proposed by the additive manufacturing
        supplier.    \nThis endpoint is used by users from the additive manufactuirng
        supplier that're not collaboration leads. The initial pricing cannot be updated."
      operationId: updates-a-production-option-proposed-by-the-additive-manufacturing-supplier----this-endpoint-is-used
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataproductiondataidbasic-put
      parameters:
      - in: body
        name: AdditionalProductionDataBasicUpdateRequest
        description: A request about updating a suppliers production option, excluding
          pricing information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: productionDataId
        description: The ID of a production option
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Suppliers
      - Production
      - Option
  /collaborationRooms/{collaborationRoomId}/productionData/confirmed:
    get:
      summary: Retrieves the confirmed production option
      description: Retrieves the production option confirmed as the finalized production
        requirements, and the initial pricing for it.
      operationId: retrieves-the-production-option-confirmed-as-the-finalized-production-requirements-and-the-initial-p
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataconfirmed-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Confirmed
      - Production
      - Option
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