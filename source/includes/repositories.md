# Repositories

## Get Repositories

```shell
$ curl "https://rodeocode.com/api/repositories/"
[
  {
    "id": 1,
    "team_id": 1,
    "created_at": "Sun, 06 Mar 2016 22:30:08 -0000"
  }
]
```

Retrieve all repos associated with the given project.

### HTTP Request

`GET https://rodeocode.com/api/repositories/`


## Get Git Repositories Associated with Project

```shell
$ curl "https://rodeocode.com/api/projects/1/repositories/"
[
  {
    "id": 1,
    "team_id": 1,
    "created_at": "Sun, 06 Mar 2016 22:30:08 -0000"
  },
  ...
]
```

Retrieve all repositories associated with the given project.

### HTTP Request

`GET https://rodeocode.com/api/projects/<projectId>/repositories/`


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
      "repository_id": 1
    },
    ...
  ]
}
```

Retrieve all pull requests for the given project.

### HTTP Request

`GET https://rodeocode.com/api/project/<project_id>/pull_requests/`

## Get Repository Pull Requests

```shell
$ curl "https://rodeocode.com/api/repositories/1/pull_requests/"
{
  "count": 2,
  "data": [
    {
      "id": 1,
      "repository_id": 1
    },
    ...
  ]
}
```

Retrieve all pull requests for the given repository.

### HTTP Request

`GET https://rodeocode.com/api/repository/<repository_id>/pull_requests/`
