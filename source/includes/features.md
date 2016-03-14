# Features

## Get Project Features

```shell
$ curl "https://rodeocode.com/api/project/1/features/"
{
    "count": 2,
    "next": null,
    "previous": null,
    "results": [
        {
            "id": 1,
            "name": "Authentication",
            "description": "Authenticate users against a database",
            "active": true,
            "created_at": "2016-03-14T08:40:37.749449Z",
            "project": 1
        },
        ...
    ]
}
```

Retrieve all features that the currently authenticated user has access to.

### HTTP Request

`GET https://rodeocode.com/api/projects/<project_id>/features/`


## Create a Feature

```shell
$ curl "https://rodeocode.com/api/projects/1/features/"
  -X POST
  -d @- <<REQUEST_BODY
{
    "name": "Logout from dashboard",
    "description": "functionality to un-authenticate the client"
}
REQUEST_BODY
```

Create a feature.

### HTTP Request

`POST https://rodeocode.com/api/projects/<project_id>/features/`


## Get a Project Feature

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/"
  -X GET
{
    "id": 1,
    "name": "Authentication",
    "description": "Authenticate users against a database",
    "active": true,
    "created_at": "2016-03-14T08:40:37.749449Z",
    "project": 1
}
```

Get an existing project feature.

### HTTP Request

`GET https://rodeocode.com/api/projects/<projectId>/features/<feature_id>/`


## Update a Project Feature

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/"
  -X PATCH
  -d @- <<REQUEST_BODY
{
    "name": "Modified name"
}
REQUEST_BODY
```

Update an existing project feature.

### HTTP Request

`PATCH https://rodeocode.com/api/projects/<projectId>/features/<feature_id>/`


## Deleting a Project Feature

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/"
  -X PATCH
  -d @- <<REQUEST_BODY
{
    "active": false
}
REQUEST_BODY
```

Delete an existing project feature.

### HTTP Request

`PATCH https://rodeocode.com/api/projects/<projectId>/features/<feature_id>/`
