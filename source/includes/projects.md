# Projects

## Get Projects

```shell
$ curl "https://rodeocode.com/api/projects/"
[
    {
        "id": 1,
        "name": "test",
        "team_id": 1,
        "repositories": [
            {
                "id": 1,
                "team_id": 1,
                "created_at": "Sun, 06 Mar 2016 22:30:08 -0000"
            },
            ...
        ],
        "created_at": "Sun, 06 Mar 2016 22:27:14 -0000"
    }
]
```

Retrieve all projects that the currently authenticated user has access to.

### HTTP Request

`GET https://rodeocode.com/api/projects/`


## Create a Project

```shell
$ curl "https://rodeocode.com/api/projects/"
  -X POST
  -d @- <<REQUEST_BODY
{
    "name": "Test"
}
REQUEST_BODY
```

Create a project.

### HTTP Request

`POST https://rodeocode.com/api/projects/`


## Get a Project

```shell
$ curl "https://rodeocode.com/api/projects/1/"
  -X GET
```

Get an existing project.

### HTTP Request

`GET https://rodeocode.com/api/projects/<projectId>/`


## Update a Project

```shell
$ curl "https://rodeocode.com/api/projects/1/"
  -X PATCH
  -d @- <<REQUEST_BODY
{
    "name": "modified project"
}
REQUEST_BODY
```

Update an existing project.

### HTTP Request

`PATCH https://rodeocode.com/api/projects/<projectId>/`


## Deleting a Project

```shell
$ curl "https://rodeocode.com/api/projects/1/"
  -X PATCH
  -d @- <<REQUEST_BODY
{
    "active": false
}
REQUEST_BODY
```

Delete an existing project.

### HTTP Request

`PATCH https://rodeocode.com/api/projects/<projectId>/`
