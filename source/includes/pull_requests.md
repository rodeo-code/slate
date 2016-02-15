# Pull Requests

## Get All Pull Requests

```shell
$ curl "https://rodeocode.com/api/pull_requests/"
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

Retrieve all pull requests that the currently authed user/API key
has access to.

### HTTP Request

`GET https://rodeocode.com/api/pull_requests/`

## Get Project Pull Requests

```shell
$ curl "https://rodeocode.com/api/projects/1/pull_requests/"
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

Retrieve all pull requests for the given project.

### HTTP Request

`GET https://rodeocode.com/api/project/<project_id>/pull_requests/`
