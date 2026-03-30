# nihonshufyi

[![crates.io](https://img.shields.io/crates/v/nihonshufyi.svg)](https://crates.io/crates/nihonshufyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Sake guide with rice varieties, breweries, and tasting notes — API client for [nihonshufyi.com](https://nihonshufyi.com).

> **Try the interactive tools at [nihonshufyi.com](https://nihonshufyi.com)**

## Install

`cargo add nihonshufyi`

## Quick Start

```rust
use nihonshufyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("dassai-23").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install nihonshufyi` | [PyPI](https://pypi.org/project/nihonshufyi/) |
| **npm** | `npm install nihonshufyi` | [npm](https://www.npmjs.com/package/nihonshufyi) |
| **Go** | `go get github.com/fyipedia/nihonshufyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/nihonshufyi-go) |
| **Rust** | `cargo add nihonshufyi` | [crates.io](https://crates.io/crates/nihonshufyi) |
| **Ruby** | `gem install nihonshufyi` | [rubygems](https://rubygems.org/gems/nihonshufyi) |

## Embed Widget

Embed [NihonshuFYI](https://nihonshufyi.com) widgets on any website with [nihonshufyi-embed](https://widget.nihonshufyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/nihonshufyi-embed@1/dist/embed.min.js"></script>
<div data-nihonshufyi="entity" data-slug="dassai-23"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.nihonshufyi.com)

## Links

- [NihonshuFYI](https://nihonshufyi.com) — Main site
- [API Documentation](https://nihonshufyi.com/developers/)
- [OpenAPI Spec](https://nihonshufyi.com/api/openapi.json)
- [Glossary](https://nihonshufyi.com/glossary/)

## License

MIT
