---
name: Auth0
x-slug: auth0
description: The new way to solve Identity
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
x-kinRank: "9"
x-alexaRank: "4820"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apis.md
specificationVersion: "0.14"
apis:
- name: Auth0 Jobs API Jobs Users Imports
  x-api-slug: auth0-jobs-api
  description: jobs users imports.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//jobs//api/v2/jobs/users-imports
  tags: Jobs,Users,Imports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2jobsusersimports-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2jobsusersimports-post-openapi.md
- name: Auth0 Jobs API
  x-api-slug: auth0-jobs-api
  description: The new way to solve Identity
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//jobs
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/openapi.md
- name: Auth0 Stats API Get Active Users
  x-api-slug: auth0-stats-api
  description: Gets the active users count (logged in during the last 30 days).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//stats//api/v2/stats/active-users
  tags: Stats,Active,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2statsactiveusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2statsactiveusers-get-openapi.md
- name: Auth0 Stats API
  x-api-slug: auth0-stats-api
  description: The new way to solve Identity
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//stats
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/openapi.md
- name: Auth0 Users API Deletes all users.
  x-api-slug: auth0-users-api
  description: Deletes all users. use with caution.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//users//api/v2/users
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2users-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2users-delete-openapi.md
- name: Auth0 Users API Gets all users who have logged in.
  x-api-slug: auth0-users-api
  description: Gets all users who have logged in..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//users//api/v2/users
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2users-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2users-get-openapi.md
- name: Auth0 Users API Creates a user.
  x-api-slug: auth0-users-api
  description: Creates a user..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//users//api/v2/users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2users-post-openapi.md
- name: Auth0 Users API Deletes a user.
  x-api-slug: auth0-users-api
  description: Deletes a user..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//users//api/v2/users/{id}
  tags: Users,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2usersid-delete-openapi.md
- name: Auth0 Users API Gets a user.
  x-api-slug: auth0-users-api
  description: Gets a user..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//users//api/v2/users/{id}
  tags: Users,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2usersid-get-openapi.md
- name: Auth0 Users API Updates a user.
  x-api-slug: auth0-users-api
  description: Updates a user..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//users//api/v2/users/{id}
  tags: Users,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2usersid-patch-openapi.md
- name: Auth0 Users API Deletes a multifactor provider for a user.
  x-api-slug: auth0-users-api
  description: Deletes a multifactor provider for a user..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//users//api/v2/users/{id}/multifactor/{provider}
  tags: Users,Id,Multifactor,Provider
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/apiv2usersidmultifactorprovider-delete-openapi.md
- name: Auth0 Users API
  x-api-slug: auth0-users-api
  description: The new way to solve Identity
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11272-auth0.jpg
  humanURL: https://auth0.com/
  baseURL: https://login.auth0.com//users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/auth0/openapi.md
x-common:
- type: x-blog
  url: https://auth0.com/blog/
- type: x-blog-rss
  url: http://feeds.feedburner.com/auth0
- type: x-crunchbase
  url: https://crunchbase.com/organization/auth0
- type: x-developer
  url: https://auth0.com/docs/apiv2
- type: x-email
  url: privacy@auth0.com
- type: x-email
  url: legal@auth0.com
- type: x-email
  url: ricky@auth0.com
- type: x-github
  url: https://github.com/auth0
- type: x-pricing
  url: https://auth0.com/pricing
- type: x-service-level-agreement
  url: https://auth0.com/docs/sla
- type: x-twitter
  url: https://twitter.com/authzero
- type: x-twitter
  url: https://twitter.com/auth0
- type: x-website
  url: https://auth0.com/
- type: x-website
  url: http://auth0.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---