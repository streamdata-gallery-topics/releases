---
swagger: "2.0"
x-collection-name: Rotten Tomatoes
x-complete: 0
info:
  title: Rotten Tomatoes Get Lists Dvds Current Releases
  description: Get lists dvds current releases.json.
  contact:
    name: Mike Ralphson
    url: https://github.com/mermade/mashery2openapi
    email: mike.ralphson@gmail.com
  version: "1.0"
host: api.rottentomatoes.com
basePath: /api/public/v1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/dvds/current_releases.json:
    get:
      summary: Get Lists Dvds Current Releases
      description: Get lists dvds current releases.json.
      operationId: getListsDvdsCurrentReleases.json
      x-api-path-slug: listsdvdscurrent-releases-json-get
      parameters:
      - in: query
        name: country
        description: Provides localized data for the selected country (ISO 3166-1
          alpha-2) if available
      - in: query
        name: page
        description: The selected page of current DVD releases
      - in: query
        name: page_limit
        description: The amount of new release dvds to show per page
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Dvds
      - Current
      - Releases
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