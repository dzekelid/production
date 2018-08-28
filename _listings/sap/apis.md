---
name: SAP
x-slug: sap
description: Get software and technology solutions from SAP, the leader in business
  applications.  Run simple with the best in cloud, analytics, mobile and IT solutions.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
x-kinRank: "8"
x-alexaRank: "1965"
tags: Production
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/apis.md
specificationVersion: "0.14"
apis:
- name: Manufacturing Network Customer APIs - Retrieves the production data
  x-api-slug: collaborationroomscollaborationroomidproductiondata-get
  description: Retrieves the production data in a collaboration room, including the
    currency, all the production options, and the initial pricings provided by the
    supplier.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondata-get-openapi.md
- name: Manufacturing Network Customer APIs - Creates a production option
  x-api-slug: collaborationroomscollaborationroomidproductiondata-post
  description: "Creates a new production option, providing the pricing information
    in the meantime.  \nThe login user must be a collaboration lead from the additive
    manufacturing supplier."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondata-post-openapi.md
- name: Manufacturing Network Customer APIs - Creates a production option without
    pricing
  x-api-slug: collaborationroomscollaborationroomidproductiondatabasic-post
  description: "Creates a new production option without an initial pricing.  \nThis
    endpoint is used by users from the additive manufactuirng supplier that're not
    collaboration leads."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondatabasic-post-openapi.md
- name: Manufacturing Network Customer APIs - Updates the customer's production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataoriginalrequirement-put
  description: "Updates the customer's production option.   \nThe login user must
    be from the customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondataoriginalrequirement-put-openapi.md
- name: Manufacturing Network Customer APIs - Updates a supplier's production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataproductiondataid-put
  description: "Updates a production option proposed by the additive manufacturing
    supplier as well as the initial pricing for this option.  \nThe login user must
    be a collaboration lead from the additive manufacturing supplier."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondataproductiondataid-put-openapi.md
- name: Manufacturing Network Customer APIs - Deletes a supplier's production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataproductiondataid-delete
  description: "Deletes a production option proposed by the additive manufacturing
    supplier. The initial pricing is deleted along with it.  \nThe login user must
    be from the additive manufacturing supplier."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondataproductiondataid-delete-openapi.md
- name: Manufacturing Network Customer APIs - Updates a supplier's production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataproductiondataidbasic-put
  description: "Updates a production option proposed by the additive manufacturing
    supplier.    \nThis endpoint is used by users from the additive manufactuirng
    supplier that're not collaboration leads. The initial pricing cannot be updated."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondataproductiondataidbasic-put-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves the confirmed production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataconfirmed-get
  description: Retrieves the production option confirmed as the finalized production
    requirements, and the initial pricing for it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondataconfirmed-get-openapi.md
- name: Manufacturing Network Customer APIs - Confirms a production option
  x-api-slug: collaborationroomscollaborationroomidproductiondataproductiondataidconfirm-post
  description: "Confirms a production option along with the initial pricing for it.
    \ \nThe production option might be proposed by the customer or the additive manufacturing
    supplier.   \nThe login user must be from the customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondataproductiondataidconfirm-post-openapi.md
- name: Manufacturing Network Customer APIs - Cancels the confirmation of a production
    option
  x-api-slug: collaborationroomscollaborationroomidproductiondataproductiondataidcancelconfirm-post
  description: "Undos the confirmation of a production option.  \nThe login user must
    be from the customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondataproductiondataidcancelconfirm-post-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves the production data
  x-api-slug: collaborationroomscollaborationroomidproductiondata-get
  description: Retrieves the production data in a collaboration room, including the
    currency, all the production options, and the initial pricings provided by the
    supplier.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/production/master/_listings/sap/collaborationroomscollaborationroomidproductiondata-get-openapi.md
x-common:
- type: x-website
  url: https://www.sap.com/index.html
- type: x-api-gallery
  url: http://santander.bank.api.gallery.streamdata.io
- type: x-api-stack
  url: http://sap.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/sap-canada
- type: x-developer
  url: https://api.sap.com/
- type: x-github
  url: https://github.com/sap
- type: x-twitter
  url: https://twitter.com/SAP
- type: x-website
  url: https://www.sap.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---