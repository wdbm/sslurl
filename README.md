# sslurl

sslurl is a URL HTTP to HTTPS redirection website. If it receives a request for a URL starting with "http://", it redirects to the URL with "http://" changed to "https://".

# setup

```Bash
pip install sslurl
```

# Flask

```Bash
while true; do
    sslurl
done
```

# Gunicorn

```Bash
gunicorn --workers=2 "sslurl.__init__:WSGI()" --bind=0.0.0.0:80
```
