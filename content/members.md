+++
title = "Members of Problem Details"
weight = 1
+++

## Members of Problem Details

### `type: string`

A URI that uniquely identifies the problem. This is used by the consumer of the API to determine which error has occurred. Different occurrences of the same type of error should use the same `type` value.

### `title: string`

A human-readable name for the problem. This should not change between different occurrences of the same type of problem. The exception is to localize the title.

### `status: number`

The HTTP status code of the response. This is included to preserve the status code in case it is changed by a proxy or cache before reaching the API consumer. It also preserves the status if the response is stored for later review, such as in a log message.

### `detail: string`

A human-readable explanation of the specific occurrence of problem. API consumers should not try to parse this for information, instead extra members should be defined (see below).

### `instance: string`

A URI that identifies the specific occurrence of the problem. This could dereference to a more detailed explanation of the specific occurrence.
