# Projects

## Get Projects

```shell
$ curl "https://rodeocode.com/api/projects/"
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

## Get Team Projects

```shell
$ curl "https://rodeocode.com/api/teams/1/projects/"
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

Retrieve all projects that the given [team](#teams) has access to.

### HTTP Request

`GET https://rodeocode.com/api/teams/<team_id>/projects/`
