# Go - Logging

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
