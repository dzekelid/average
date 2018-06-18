---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Rates Get Daily Average
  description: Returns a daily average rate as of a specific date
  version: 1.0.0
host: www.xignite.com
basePath: xRates.json/XigniteRates
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetAverageRate:
    get:
      summary: Get Average Rate
      description: Returns an average rate as of a specific date.
      operationId: postGetaveragerate
      x-api-path-slug: getaveragerate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Average
      - Rate
  /GetAverageRates:
    get:
      summary: Get Average Rates
      description: Returns average rate for a period.
      operationId: postGetaveragerates
      x-api-path-slug: getaveragerates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Average
      - Rates
  /GetRateMovingAverage:
    get:
      summary: Get Rate Moving Average
      description: Returns a moving  average rate as of a specific date
      operationId: postGetratemovingaverage
      x-api-path-slug: getratemovingaverage-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Moving
      - Average
  /GetDailyAverage:
    get:
      summary: Get Daily Average
      description: Returns a daily average rate as of a specific date
      operationId: postGetdailyaverage
      x-api-path-slug: getdailyaverage-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Daily
      - Average
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