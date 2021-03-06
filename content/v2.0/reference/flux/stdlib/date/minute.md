---
title: date.minute() function
description: >
  The `date.minute()` function returns the minute of a specified time.
  Results range from `[0-59]`.
aliases:
  - /v2.0/reference/flux/functions/date/minute/
menu:
  v2_0_ref:
    name: date.minute
    parent: Date
weight: 301
---

The `date.minute()` function returns the minute of a specified time.
Results range from `[0-59]`.

_**Function type:** Transformation_  

```js
import "date"

date.minute(t: 2019-07-17T12:05:21.012Z)

// Returns 5
```

## Parameters

### t
The time to operate on.

_**Data type:** Time_
