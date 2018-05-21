---
swagger: "2.0"
x-collection-name: Alpha Vantage
x-complete: 0
info:
  title: Alpha Vantage Exponential Moving Average (EMA)
  description: This API returns the exponential moving average (EMA)
  version: 1.0.0
host: www.alphavantage.co
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query?function=SMA:
    get:
      summary: Simple Moving Average (SMA)
      description: This API returns the simple moving average (SMA) values.
      operationId: getSimpleMovingAverage
      x-api-path-slug: queryfunctionsma-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: series_type
        description: The desired price type in the time series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      - in: query
        name: time_period
        description: Number of data points used to calculate each moving average value
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Simple Moving Average
      - SMA
  /query?function=EMA:
    get:
      summary: Exponential Moving Average (EMA)
      description: This API returns the exponential moving average (EMA)
      operationId: getExponentialMovingAverage
      x-api-path-slug: queryfunctionema-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: series_type
        description: The desired price type in the time series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      - in: query
        name: time_period
        description: Number of data points used to calculate each moving average value
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Exponential Moving Average
      - EMA
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