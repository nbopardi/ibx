# Login

The smallest possible IBX program: connect, wait for `next_valid_id`, disconnect.

## What this shows

- Reading credentials from environment variables.
- Calling `EClient.connect(...)` against the paper host.
- Receiving `next_valid_id` — the signal that the session is fully established and ready for requests.

## Run it

```bash
IB_USERNAME=... IB_PASSWORD=... python examples/hello_login.py
```

## Source

```python
{{#include ../../../../../examples/hello_login.py}}
```
