---
swagger: "2.0"
x-collection-name: Alpha Vantage
x-complete: 1
info:
  title: Alpha Vantage
  description: alpha-vantage-apis-are-grouped-into-four-categories-1-stock-time-series-data-2-physical-and-digitalcrypto-currencies-e-g--bitcoin-3-stock-technical-indicators-and-4-sector-performances--all-apis-are-realtime-the-latest-data-points-are-derived-from-the-current-trading-day--
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
  /query?function=MACD:
    get:
      summary: Moving Average Convergence / Divergence (MACD)
      description: This API returns the moving average convergence / divergence (MACD)
        values.
      operationId: getMovingAverageConvergenceDivergence
      x-api-path-slug: queryfunctionmacd-get
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
      - Moving Average Convergence
      - MACD
  /query?function=ADX:
    get:
      summary: Average Directional Movement Index (ADX)
      description: This API returns the average directional movement index (ADX) values.
      operationId: getAverageDirectionalMovementIndex
      x-api-path-slug: queryfunctionadx-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
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
      - Average Directional Movement Index
      - ADX
---