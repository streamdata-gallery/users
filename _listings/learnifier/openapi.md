---
swagger: "2.0"
x-collection-name: Learnifier
x-complete: 1
info:
  title: Learnifier
  version: 1.1.0
host: learnifier.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /extuser:
    get:
      summary: Gets a user by external id
      description: Gets a user by external id.
      operationId: extuser.get
      x-api-path-slug: extuser-get
      parameters:
      - in: query
        name: extid
        description: The external id of the user
      responses:
        200:
          description: OK
      tags:
      - Users
  /globalusergroups:
    get:
      summary: List Global User Groups.
      description: Returns a list of Global User Groups. Global User Groups are set
        up for the realm, and will generate groups that can be used on the client
        level.
      operationId: globalusergroups.get
      x-api-path-slug: globalusergroups-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /globalusergroups/{groupid}/members:
    get:
      summary: List of all users in group.
      description: Returns a list of all members in User Groups that are based on
        the Global Group with this groupid.
      operationId: globalusergroups.groupid.members.get
      x-api-path-slug: globalusergroupsgroupidmembers-get
      parameters:
      - in: path
        name: groupid
        description: ID of group
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /orgunits/{orgid}/usergroups:
    get:
      summary: List User Groups.
      description: Returns a list of User Groups for the org unit.
      operationId: orgunits.orgid.usergroups.get
      x-api-path-slug: orgunitsorgidusergroups-get
      parameters:
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Users
      - Groups
    post:
      summary: Create a User Group.
      description: Create a User Group.
      operationId: orgunits.orgid.usergroups.post
      x-api-path-slug: orgunitsorgidusergroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Users
      - Groups
  /orgunits/{orgid}/usergroups/{groupid}:
    get:
      summary: Get user group
      description: Returns single User Group.
      operationId: orgunits.orgid.usergroups.groupid.get
      x-api-path-slug: orgunitsorgidusergroupsgroupid-get
      parameters:
      - in: path
        name: groupid
        description: ID of group
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Users
      - Groups
      - Groupid
  /users:
    get:
      summary: Lists all users
      description: Lists all users. Only api callers that have full access can call
        this method.
      operationId: users.get
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of users to return
      - in: query
        name: offset
        description: The offset to start listing users from
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Adds a user
      description: Adds a user. No two users can have the same email address. Email
        is saved WITH case but compared regardless of case. Email can be changed for
        a user assuming it doesn't cause a conflict.
      operationId: users.post
      x-api-path-slug: users-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{userid}:
    get:
      summary: User information
      description: Returns information about a user
      operationId: users.userid.get
      x-api-path-slug: usersuserid-get
      parameters:
      - in: path
        name: userid
        description: A user id
      responses:
        200:
          description: OK
      tags:
      - Users
    patch:
      summary: Updates user information
      description: Updates a user. All values that have a key defined in the input
        will be set. So if a value should not be updated omit it totally from the
        input, otherwise it will be unset.
      operationId: users.userid.patch
      x-api-path-slug: usersuserid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{userid}/pic?key={APIKEY}:
    get:
      summary: User profile picture
      description: |-
        Returns a thumbnail picture of the user. This can either be a selected picture or an auto generated image. This method doesn't require a full sign in. The api key is sufficient.
        The image is square and is likely, but not necessary, to be in 128x128 PNG format. However the format will always be either PNG, JPEG or GIF.
      operationId: users.userid.pic_key_APIKEY.get
      x-api-path-slug: usersuseridpickeyapikey-get
      parameters:
      - in: path
        name: APIKEY
      - in: path
        name: userid
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{userid}/projectParticipations:
    get:
      summary: Returns information about the projects the user is a participant in.
      description: Returns information about the projects the user is a participant
        in. Only the projects that the current token have access to will be listed.
      operationId: users.userid.projectParticipations.get
      x-api-path-slug: usersuseridprojectparticipations-get
      parameters:
      - in: path
        name: userid
        description: A user id
      responses:
        200:
          description: OK
      tags:
      - Users
---