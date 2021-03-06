---
name: Google People
description: The People API lets you list authenticated users Contacts and retrieve
  profile information for authenticated users and their contacts. For example, lets
  say the authenticated user, Jen, has Fabian and Ranjith in her private contacts.
  When your app calls people.connections.list to retrieve a list of her connections,
  Jen is presented with a consent screen asking to give the app access to the list.
  If Jen consents, the app retrieves a list containing Fabian and Ranjith (with a
  resource name for each person). The app can then call people.get, passing in a resource
  name, to get private contact and public profile data for each person.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-people.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Users
- Stack Network
- People
- Google APIs
created: "2018-03-10"
modified: "2018-03-10"
url: https://raw.githubusercontent.com/streamdata-gallery/users/master/_listings/google-people/apis.yaml
specificationVersion: "0.14"
apis: []
x-common:
- type: x-code
  url: https://developers.google.com/people/v1/libraries
- type: x-terms-of-service
  url: https://developers.google.com/people/terms
- type: x-website
  url: https://developers.google.com/people/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---