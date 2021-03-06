---
title: Delete a token
seotitle: Delete an authentication token from InfluxDB
description: Delete an authentication token from InfluxDB using the InfluxDB UI or the `influx` CLI.
aliases:
  - /v2.0/users/tokens/delete-token
menu:
  v2_0:
    name: Delete a token
    parent: Manage tokens
weight: 204
---

Delete authentication tokens from the InfluxDB user interface (UI) or the `influx` command line interface (CLI).
Once deleted, all users and external integrations using the token will no longer
have access to your InfluxDB instance.

## Delete tokens in the InfluxDB UI

1. Click the Click the **Load Data** icon in the navigation bar.

    {{< nav-icon "disks" >}}

2. Click **Tokens**. All of your account's tokens appear.
3. Hover over the token you want to delete and click **Delete** and **Confirm**.

## Delete tokens using the influx CLI

Use the [`influx auth delete` command](/v2.0/reference/cli/influx/auth/delete)
to delete a token.

_This command requires an auth ID, which is available in the output of `influx auth find`._

```sh
# Syntax
influx auth delete -i <auth-id>

# Example
influx auth delete -i 03a2bee5a9c9a000
```
