---
title: influx org delete
description: The 'influx org delete' command deletes an organization in InfluxDB.
menu:
  v2_0_ref:
    name: influx org delete
    parent: influx org
weight: 201
---

The `influx org delete` command deletes an organization in InfluxDB.

## Usage
```
influx org delete [flags]
```

## Flags
| Flag             | Description                           | Input type  | {{< cli/mapped >}}    |
|:----             |:-----------                           |:----------: |:------------------    |
| `-h`, `--help`   | Help for the `delete` command         |             |                       |
| `--hide-headers` | Hide table headers (default `false`)  |             | `INFLUX_HIDE_HEADERS` |
| `-i`, `--id`     | **(Required)** Organization ID        | string      | `INFLUX_ORG_ID`       |
| `--json`         | Output data as JSON (default `false`) |             | `INFLUX_OUTPUT_JSON`  |

{{% cli/influx-global-flags %}}
