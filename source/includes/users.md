# Users

## Get Self

```shell
$ curl "https://rodeocode.com/api/accounts/self"
{
  "id": 1,
  "email": "sample@rodeocode.com"
},
```

Retrieve user metadata for the currently authed user/API key.

### HTTP Request

`GET https://rodeocode.com/api/accounts/self`

## Get Users

```shell
$ curl "https://rodeocode.com/api/users/"
{
  "count": 35,
  "data": [
    {
      "id": 1,
      "name": "rodeo-code/slate"
    },
    ...
  ]
}
```

Retrieve all users that the currently authed user/API key
has access to.

### HTTP Request

`GET https://rodeocode.com/api/users/`
