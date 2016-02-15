# Teams

## Get Teams

```shell
$ curl "https://rodeocode.com/api/teams/"
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

Retrieve all teams that the currently authed user/API key
has access to.

### HTTP Request

`GET https://rodeocode.com/api/teams/`
