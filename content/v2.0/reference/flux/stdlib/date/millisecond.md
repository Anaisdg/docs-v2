---
title: date.millisecond() function
description: >
  The `date.millisecond()` function returns the millisecond of a specified time.
  Results range from `[0-999999]`.
aliases:
  - /v2.0/reference/flux/functions/date/millisecond/
menu:
  v2_0_ref:
    name: date.millisecond
    parent: Date
weight: 301
---

The `date.millisecond()` function returns the millisecond of a specified time.
Results range from `[0-999]`.

_**Function type:** Transformation_  

```js
import "date"

date.millisecond(t: 2019-07-17T12:05:21.012934584Z)

// Returns 12
```

## Parameters

### t
The time to operate on.

_**Data type:** Time_
