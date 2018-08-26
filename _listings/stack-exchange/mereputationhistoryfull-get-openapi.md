---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange My Reputation History Full
  description: "Returns user's full reputation history, including private events.\n
    \n This method requires an access_token, with a scope containing \"private_info\".\n
    \nThis method returns a list of reputation_history."
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