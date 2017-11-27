# Raxx.MethodOverride

**[Raxx](https://github.com/crowdhailer/raxx) middleware to override a request's `POST` method with value declared in `_method` query parameter.**

[![Hex pm](http://img.shields.io/hexpm/v/raxx_method_override.svg?style=flat)](https://hex.pm/packages/raxx_method_override)
[![Build Status](https://secure.travis-ci.org/CrowdHailer/raxx_method_override.svg?branch=master
"Build Status")](https://travis-ci.org/CrowdHailer/raxx_method_override)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

- [Install from hex.pm](https://hex.pm/packages/raxx_method_override)
- [Documentation available on hexdoc](https://hexdocs.pm/raxx_method_override)
- [Raxx discussion on slack](https://elixir-lang.slack.com/messages/C56H3TBH8/)

## Getting Started

Override request methods in any Raxx Server module.

```elixir
defmodule MyApp.WWW do
  use Raxx.Server
  use Raxx.MethodOverride

  @impl Raxx.Server
  def handle_request(request, state) do
  # ...
end
```
