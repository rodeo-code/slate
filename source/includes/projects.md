# Projects

```shell
$ curl "https://rodeocode.com/api/projects/"
```

> Returns JSON by default:

```
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

Retrieve all projects that the currently authed user/API key
has access to.

### HTTP Request

`GET https://rodeocode.com/api/projects/`
