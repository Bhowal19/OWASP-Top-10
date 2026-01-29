# Code-Level Examples

SSRF often appears in simple, well-intentioned code.

Consider a URL fetch feature.

```python
import requests

def fetch_resource(url):
    return requests.get(url).content
