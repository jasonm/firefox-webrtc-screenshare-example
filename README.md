See https://github.com/muaz-khan/Firefox-Extensions/issues/4 for reference.

Generate a local cert so you can serve via HTTPS locally:

```bash
openssl req -new -x509 -keyout localhost.pem -out localhost.pem -days 365 -nodes
```

Then `python serve.py` and visit https://localhost:4443/index.html
