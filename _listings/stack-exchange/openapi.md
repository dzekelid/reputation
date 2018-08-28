swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 1
info:
  title: Stack Exchange
  description: stack-exchange-is-a-network-of-130-qa-communities-including-stack-overflow-
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/reputation:
    get:
      summary: My Reputation
      description: "Returns the reputation changed for the user associated with the
        given access_token.\n \nThis method returns a list of reputation changes."
      operationId: returns-the-reputation-changed-for-the-user-associated-with-the-given-access-token-this-method-retur
      x-api-path-slug: mereputation-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Reputation
  /me/reputation-history:
    get:
      summary: My Reputation History
      description: "Returns user's public reputation history.\n \nThis method returns
        a list of reputation_history."
      operationId: returns-users-public-reputation-history-this-method-returns-a-list-of-reputation-history
      x-api-path-slug: mereputationhistory-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Reputation
  /me/reputation-history/full:
    get:
      summary: My Reputation History Full
      description: "Returns user's full reputation history, including private events.\n
        \n This method requires an access_token, with a scope containing \"private_info\".\n
        \nThis method returns a list of reputation_history."
      operationId: returns-users-full-reputation-history-including-private-events--this-method-requires-an-access-token
      x-api-path-slug: mereputationhistoryfull-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Reputation
  /users/{ids}/reputation:
    get:
      summary: Get User Reputation
      description: "Gets a subset of the reputation changes for users in {ids}.\n
        \nReputation changes are intentionally scrubbed of some data to make it difficult
        to correlate votes on particular posts with user reputation changes. That
        being said, this method returns enough data for reasonable display of reputation
        trends.\n \n{ids} can contain up to 100 semicolon delimited ids, to find ids
        programatically look for user_id on user or shallow_user objects.\n \nThis
        method returns a list of reputation objects."
      operationId: gets-a-subset-of-the-reputation-changes-for-users-in-ids-reputation-changes-are-intentionally-scrubb
      x-api-path-slug: usersidsreputation-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Reputation
  /users/{ids}/reputation-history:
    get:
      summary: Get User Reputation History
      description: "Returns users' public reputation history.\n \nThis method returns
        a list of reputation_history."
      operationId: returns-users-public-reputation-history-this-method-returns-a-list-of-reputation-history
      x-api-path-slug: usersidsreputationhistory-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Reputation
      - History
  /users/{id}/reputation-history/full:
    get:
      summary: Get User Reputation History Full
      description: "Returns a user's full reputation history, including private events.\n
        \nThis method requires an access_token, with a scope containing \"private_info\".\n
        \nThis method returns a list of reputation_history."
      operationId: returns-a-users-full-reputation-history-including-private-events-this-method-requires-an-access-toke
      x-api-path-slug: usersidreputationhistoryfull-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Reputation