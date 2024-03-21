# party

[![Package Version](https://img.shields.io/hexpm/v/party)](https://hex.pm/packages/party)
[![Hex Docs](https://img.shields.io/badge/hex-docs-ffaff3)](https://hexdocs.pm/party/)

A little parser combinator library for Gleam!

A little demo:
```gleam
fn identstring() -> Parser(String, e) {
  use first <- do(lowercase_letter())
  use rest <- do(many_concat(either(alphanum(), char("_"))))
  return(first <> rest)
}
```

## Installation

If available on Hex this package can be added to your Gleam project:

```sh
gleam add party
```

and its documentation can be found at <https://hexdocs.pm/party>.
