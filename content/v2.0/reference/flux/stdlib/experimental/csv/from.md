---
title: csv.from() function
description: >
  The experimental `csv.from()` function retrieves annotated CSV from a URL.
menu:
  v2_0_ref:
    name: csv.from *
    parent: CSV-exp
weight: 401
---

The experimental `csv.from()` function retrieves [annotated CSV](/v2.0/reference/syntax/annotated-csv/) **from a URL**.

{{% note %}}
The experimental `csv.from()` function is an alternative to the standard
[`csv.from()` function](/v2.0/reference/flux/stdlib/csv/from/).
{{% /note %}}

_**Function type:** Input_

```js
import "experimental/csv"

csv.from(url: "http://localhost:9999/")
```

## Parameters

### url
The URL to retrieve annotated CSV from.

_**Data type:** String_


## Examples

##### Query annotated CSV data from a remote URL
```js
import "experimental/csv"

csv.from(url: "http://mydomain.com/csv/example.csv")
  |> filter(fn: (r) => r._measurement == "example-measurement")
```

## Function definition
```js
package csv

import c "csv"
import "experimental/http"

from = (url) => c.from(csv: string(v: http.get(url: url).body))
```
