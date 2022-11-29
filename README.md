# go-json

A fork of `encoding/json` from go's stdlib which contains an extra Decoder function which enforces strict field name
matching. This is currently only tested in practice not in any specific unit tests.

## Requirements

- go 1.18
  - use of `any` type alias

## Changes

- Addition of function `UseStrictNames` to `Decoder` in 5d7d407
  - Adjusts the  `strict` boolean field of the `decodeState` struct to be `true` for that specific `Decoder`
  - The `strict` field determines if the `field` function `equalFold` is used when matching struct fields

## Fork

Forked initially from [1.19.3] commit sha1 [5d5ed57b134b7a02259ff070864f753c9e601a18].

## Versioning

The following table contains a list of tags for this repository and their go version equivalence.

|   Tag    | Go Version |                 Go Commit                  |
|:--------:|:----------:|:------------------------------------------:|
| [v0.1.0] |  [1.19.3]  | [5d5ed57b134b7a02259ff070864f753c9e601a18] |


[v0.1.0]: https://github.com/james-d-elliott/go-json/releases/tag/v0.1.0

[1.19.3]: https://github.com/golang/go/tree/go1.19.3/src/encoding/json

[5d5ed57b134b7a02259ff070864f753c9e601a18]: https://github.com/golang/go/commit/5d5ed57b134b7a02259ff070864f753c9e601a18