# Repos

## Get All Repos

```shell
$ curl "https://rodeocode.com/api/repos/"
{
  "count": 2,
  "data": [
    {
      "id": 1,
      "project_id": 1
    },
    ...
  ]
}
```

Retrieve all repos that the currently authed user/API key
has access to.

### HTTP Request

`GET https://rodeocode.com/api/repos/`

## Get Project Repos

```shell
$ curl "https://rodeocode.com/api/projects/1/repos/"
{
  "count": 2,
  "data": [
    {
      "id": 1,
      "project_id": 1
    },
    ...
  ]
}
```

Retrieve all repos for the given project.

### HTTP Request

`GET https://rodeocode.com/api/project/<project_id>/repos/`
