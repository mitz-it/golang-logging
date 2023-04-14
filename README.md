# Go - Logging

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=mitz-it_golang-logging&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=mitz-it_golang-logging) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=mitz-it_golang-logging&metric=coverage)](https://sonarcloud.io/summary/new_code?id=mitz-it_golang-logging)

Abstraction over [zero](https://github.com/rs/zerolog) for logging.

## Installation

```bash
  go get -u github.com/mitz-it/golang-logging
```

## Usage 1

```go
package main

import "github.com/mitz-it/golang-logging"

func main() {
  logger := logging.NewLogger()

  msg := "world"
  logger.Standard.Info().Msgf("hello %s", world)
}
```

## Usage 2

```go
package main

import "github.com/mitz-it/golang-logging"

func main() {
  msg := "world"
  logger.Log.Standard.Info().Msgf("hello %s", world)
}
```
