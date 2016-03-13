# Users

## Get Self

```shell
$ curl "https://rodeocode.com/api/accounts/self"
{
  "id": 1,
  "email": "sample@rodeocode.com",
  "created_at": "Sun, 06 Mar 2016 16:56:37 -0000"
},
```

Retrieve user metadata for the currently authed user/API key.

### HTTP Request

`GET https://rodeocode.com/api/accounts/self`


## Get Current User's Team

```shell
$ curl "https://rodeocode.com/api/accounts/teams/"
{
    "id": 1,
    "owner_id": 1,
    "members": [
        {
            "id": 1,
            "email": "sample@rodeocode.com",
            "created_at": "Sun, 06 Mar 2016 16:56:37 -0000"
        }
    ],
    "plan_id": 0,
    "created_at": "Sun, 06 Mar 2016 21:43:17 -0000"
}
```

Retrieve the team that the currently authed user/API key has access to.

### HTTP Request

`GET https://rodeocode.com/api/accounts/teams`


## Get a Team

```shell
$ curl "https://rodeocode.com/api/accounts/teams/1/"
{
    "id": 1,
    "email": "sample@rodeocode.com",
    "created_at": "Sun, 06 Mar 2016 16:56:37 -0000"
}
```

Retrieve the team that the currently authed user/API key has access to.

### HTTP Request

`GET https://rodeocode.com/api/accounts/teams`
