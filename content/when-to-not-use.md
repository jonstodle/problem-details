+++
title = "When Not To Use Problem Details"
weight = 3
+++

## When Not To Use Problem Details

When an HTTP Status Code is able to convey enough meaning by itself, no new problem details is necessary. If you want to keep consistency with other types of errors, the recommended solution is to omit the `type` field or set it to `about:blank` to indicate not specific information is available for the error. The `title` field should be set to the status phrase of the status, e.g. "Not Found" for status code `404`.
