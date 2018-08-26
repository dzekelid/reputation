---
name: Stack Exchange
x-slug: stack-exchange
description: After someone asks a question, members of the community propose answers.
  Others vote on those answers. Very quickly, the answers with the most votes rise
  to the top. You dont have to read through a lot of discussion to find the best answer.    Like
  to...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
x-kinRank: "8"
x-alexaRank: "126"
tags: Reputation
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange - My Reputation
  x-api-slug: mereputation-get
  description: "Returns the reputation changed for the user associated with the given
    access_token.\n \nThis method returns a list of reputation changes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/mereputation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/mereputation-get-openapi.md
- name: Stack Exchange - My Reputation History
  x-api-slug: mereputationhistory-get
  description: "Returns user's public reputation history.\n \nThis method returns
    a list of reputation_history."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/mereputationhistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/mereputationhistory-get-openapi.md
- name: Stack Exchange - My Reputation History Full
  x-api-slug: mereputationhistoryfull-get
  description: "Returns user's full reputation history, including private events.\n
    \n This method requires an access_token, with a scope containing \"private_info\".\n
    \nThis method returns a list of reputation_history."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/mereputationhistoryfull-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/mereputationhistoryfull-get-openapi.md
- name: Stack Exchange - Get User Reputation
  x-api-slug: usersidsreputation-get
  description: "Gets a subset of the reputation changes for users in {ids}.\n \nReputation
    changes are intentionally scrubbed of some data to make it difficult to correlate
    votes on particular posts with user reputation changes. That being said, this
    method returns enough data for reasonable display of reputation trends.\n \n{ids}
    can contain up to 100 semicolon delimited ids, to find ids programatically look
    for user_id on user or shallow_user objects.\n \nThis method returns a list of
    reputation objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/usersidsreputation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/usersidsreputation-get-openapi.md
- name: Stack Exchange - Get User Reputation History
  x-api-slug: usersidsreputationhistory-get
  description: "Returns users' public reputation history.\n \nThis method returns
    a list of reputation_history."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/usersidsreputationhistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/usersidsreputationhistory-get-openapi.md
- name: Stack Exchange - Get User Reputation History Full
  x-api-slug: usersidreputationhistoryfull-get
  description: "Returns a user's full reputation history, including private events.\n
    \nThis method requires an access_token, with a scope containing \"private_info\".\n
    \nThis method returns a list of reputation_history."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Citations, Answers, Code, Content, My API Stack, Imports, Stack, Media, Forums,
    Streams, Plugins, Questions, General Data, Relative Data, Service API, Pedestal,
    Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/usersidreputationhistoryfull-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reputation/master/_listings/stack-exchange/usersidreputationhistoryfull-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://square.api.gallery.streamdata.io
- type: x-api-stack
  url: http://stack.exchange.stack.network
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-crunchbase
  url: https://crunchbase.com/organization/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: legal@stackexchange.com
- type: x-email
  url: team@stackexchange.com
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-linkedin
  url: https://www.linkedin.com/company/stack-exchange
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: http://stackexchange.com
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---