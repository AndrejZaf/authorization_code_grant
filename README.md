## oauth2-authorization-grant
There's no ResourceServer. Just plain authorization-server

For testing purposes here's a link, log in here
http://localhost:8080/oauth/authorize?response_type=code&client_id=fooClientIdPassword2&redirect_uri=http://localhost:8080/home/&scope=read


After you receive a code (Look in the URL after log in) call the following 

localhost:8080/oauth/token

With the following body as x-www-form-urlencoded
```
grant_type - authorization_code
client_id - fooClientIdPassword2
code - M6mZo6
client_secret - secret
redirect_uri - http://localhost:8080/home
```

# Optional
## The following example already uses JWT Tokens for granting access instead of UID tokens
