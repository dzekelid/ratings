swagger: "2.0"
x-collection-name: Intrinio
x-complete: 1
info:
  title: Intrinio
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyst_ratings:
    get:
      summary: Analyst Ratings
      description: Returns analyst buy/sell/hold ratings for a specific security and
        date, as well as target prices.
      operationId: analyst-ratings
      x-api-path-slug: analyst-ratings-get
      parameters:
      - in: query
        name: action
        description: The analyst action (see section below)
        type: string
      - in: query
        name: analyst_firm_id
        description: The ID of the analyst firm
        type: string
      - in: query
        name: analyst_id
        description: The ID of the analyst
        type: string
      - in: query
        name: identifier
        description: 'the identifier for the legal entity or a security associated
          with the company:'
        type: string
      - in: query
        name: page_number
        description: an integer greater than or equal to 1 for specifying the page
          number for the return values
        type: string
      - in: query
        name: page_size
        description: an integer greater than 1 for specifying the number of results
          on each page
        type: string
      - in: query
        name: rating
        description: The analyst rating (see section below)
        type: string
      - in: query
        name: sector
        description: The name of the sector
        type: string
      - in: query
        name: source
        description: 'The source of the data: tip'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Analyst Ratings