---
title: strings.toTitle() function
description: The strings.toTitle() function converts all characters in a string to title case.
aliases:
  - /v2.0/reference/flux/functions/strings/totitle/
menu:
  v2_0_ref:
    name: strings.toTitle
    parent: Strings
weight: 301
related:
  - /v2.0/reference/flux/stdlib/strings/toupper
  - /v2.0/reference/flux/stdlib/strings/tolower
  - /v2.0/reference/flux/stdlib/strings/title
---

The `strings.toTitle()` function converts all characters in a string to title case.

_**Output data type:** String_

```js
import "strings"

strings.toTitle(v: "a flux of foxes")

// returns "A FLUX OF FOXES"
```

## Parameters

### v
The string value to convert.

_**Data type:** String_

## Examples

###### Covert characters in a string to title case
```js
import "strings"

data
  |> map(fn: (r) => ({ r with pageTitle: strings.toTitle(v: r.pageTitle) }))
```

{{% note %}}
#### The difference between toTitle and toUpper
The results of `toTitle()` and `toUpper` are often the same, however the difference
is visible with special characters:

```js
str = "ǳ"

strings.toTitle(v: str) // Returns ǲ
strings.toUpper(v: str) // Returns Ǳ
```
{{% /note %}}
