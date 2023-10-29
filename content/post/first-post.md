+++
title = 'First Post'
date = 2023-10-29T11:18:19-04:00
draft = false
description = "First Post Description"
tags = ["test-tag"]
categories = ["test-category"]
series = ["test-series"]
aliases = ["test-aliases"]
+++

# H1 - First Post

## H2 - First Post

### H3 - First Post

#### H4 - First Post

##### H5 - First Post

###### H6 - First Post

Lorem ipsum dolor sit amet, consectetur adipisici elit

## A Link

[A link](https://en.wikipedia.org/wiki/Lorem_ipsum)

## Table

| Col 1 | Col 2 | Col 3 |
| --- | --- | --- |
| Row 1 | is | here |
| This | be | row2 |

## Lists

- Dashed list
  - Indentet
- Row2
- Row3

1. Numbered list
2. goes
3. here

## Code Block Test - Python

```python
from binascii import unhexlify

# comment
b = unhexlify("BAADF00D")
if b != b"\x00":
  print(f"b is {b}")
```

## Highlight Shortcode Test - Go

{{< highlight go "linenos=table,hl_lines=8 15-17,linenostart=199" >}}
// GetTitleFunc returns a func that can be used to transform a string to
// title case.
//
// The supported styles are
//
// - "Go" (strings.Title)
// - "AP" (see https://www.apstylebook.com/)
// - "Chicago" (see https://www.chicagomanualofstyle.org/home.html)
//
// If an unknown or empty style is provided, AP style is what you get.
func GetTitleFunc(style string) func(s string) string {
  switch strings.ToLower(style) {
  case "go":
    return strings.Title
  case "chicago":
    return transform.NewTitleConverter(transform.ChicagoStyle)
  default:
    return transform.NewTitleConverter(transform.APStyle)
  }
}
{{< / highlight >}}

## Mermaid Test - Dark Theme

```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```


