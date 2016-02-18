# Organizations

## Get Organizations

```shell
$ curl "https://rodeocode.com/api/organizations/"
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

Retrieve all organizations that the currently authed user/API key
has access to.

### HTTP Request

`GET https://rodeocode.com/api/organizations/`
