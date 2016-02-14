# Authentication

The RodeoCode supports two types of authentication of requests:

- Session + CSRF cookies (standard)
- API keys supplied via HTTP header (e.g. `Authorization: meowmeowmeow`)

## Cookies

```shell
curl "https://rodeocode.com/login"
  -X POST
  -d @- <<REQUEST_BODY
{
    "email": "user@domain.com",
    "password": "12345"
}
REQUEST_BODY
```

To obtain session + CSRF tokens, access the `login` API endpoint.

`/login/`

## JWT API keys

"JWT" refers to [JSON web tokens](https://jwt.io/). *Not available yet.*
