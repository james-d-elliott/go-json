# go-json

A fork of `encoding/json` from go's stdlib which contains an extra Decoder function which enforces strict field name
matching.

## Requirements

- go 1.18
  - use of `any` type alias

## Fork

Forked initially from [go1.19.3] commit sha1 [5d5ed57b134b7a02259ff070864f753c9e601a18].


[go1.19.3]: https://github.com/golang/go/tree/go1.19.3/src/encoding/json
[5d5ed57b134b7a02259ff070864f753c9e601a18]: https://github.com/golang/go/commit/5d5ed57b134b7a02259ff070864f753c9e601a18