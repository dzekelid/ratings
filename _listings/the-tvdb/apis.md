---
name: The TVDB
x-slug: the-tvdb
description: TheTVDB.com is a community driven database of television shows. All content
  and images on the site have been contributed by the sites users; the site uses moderated
  editing to maintain its own standards. The database schema and website are open
  source under the GNU General Public License.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
x-kinRank: "7"
x-alexaRank: "0"
tags: Ratings
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/ratings/master/_listings/the-tvdb/apis.md
specificationVersion: "0.14"
apis:
- name: The TVDB API v2 - Get User Ratings
  x-api-slug: userratings-get
  description: Returns an array of ratings for the given user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/ratings/master/_listings/the-tvdb/userratings-get-openapi.md
- name: The TVDB API v2 - Get User Ratings Query
  x-api-slug: userratingsquery-get
  description: Returns an array of ratings for a given user that match the query.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/ratings/master/_listings/the-tvdb/userratingsquery-get-openapi.md
- name: The TVDB API v2 - Get User Ratings Query Params
  x-api-slug: userratingsqueryparams-get
  description: Returns a list of query params for use in the `/user/ratings/query`
    route.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/ratings/master/_listings/the-tvdb/userratingsqueryparams-get-openapi.md
- name: The TVDB API v2 - Delete User Ratings Itemtype Itemid
  x-api-slug: userratingsitemtypeitemid-delete
  description: This route deletes a given rating of a given type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/ratings/master/_listings/the-tvdb/userratingsitemtypeitemid-delete-openapi.md
- name: The TVDB API v2 - Put User Ratings Itemtype Itemid Itemrating
  x-api-slug: userratingsitemtypeitemiditemrating-put
  description: This route updates a given rating of a given type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/ratings/master/_listings/the-tvdb/userratingsitemtypeitemiditemrating-put-openapi.md
x-common:
- type: x-api-gallery
  url: http://the.open.movie.database.api.gallery.streamdata.io
- type: x-api-stack
  url: http://the.tvdb.stack.network
- type: x-documentation
  url: https://api.thetvdb.com/swagger
- type: x-website
  url: http://thetvdb.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---