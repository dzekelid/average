---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite Rates
  description: provide-information-about-interest-rates
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
    post:
      summary: Get Average Rate
      description: Returns an average rate as of a specific date.
      operationId: postGetaveragerate
      x-api-path-slug: getaveragerate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Average
      - Rate
  /GetAverageRates:
    post:
      summary: Get Average Rates
      description: Returns average rate for a period.
      operationId: postGetaveragerates
      x-api-path-slug: getaveragerates-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Average
      - Rates
  /GetRateMovingAverage:
    post:
      summary: Get Rate Moving Average
      description: Returns a moving  average rate as of a specific date
      operationId: postGetratemovingaverage
      x-api-path-slug: getratemovingaverage-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Rate
      - Moving
      - Average
  /GetDailyAverage:
    post:
      summary: Get Daily Average
      description: Returns a daily average rate as of a specific date
      operationId: postGetdailyaverage
      x-api-path-slug: getdailyaverage-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Daily
      - Average
  /GetMonthlyTreasuryAverage:
    post:
      summary: Get Monthly Treasury Average
      description: Returns a daily average rate as of a specific date
      operationId: postGetmonthlytreasuryaverage
      x-api-path-slug: getmonthlytreasuryaverage-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monthly
      - Treasury
      - Average
---