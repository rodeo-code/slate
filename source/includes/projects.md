# Projects

## Get Projects

```shell
$ curl "https://rodeocode.com/api/projects/"
{
    "count": 45,
    "next": "https://rodeocode.com/api/projects/?page=2",
    "previous": null,
    "results": [
        {
            "id": 1,
            "name": "RodeoCode admin",
            "slug": "rodeocode-admin",
            "active": true,
            "created_at": "2016-03-12T07:53:24Z",
            "team": 1,
            "repositories": [
                1
            ]
        },
        ...
    ]
}
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


## Search Projects

```shell
$ curl "https://rodeocode.com/api/projects/?q=admin"
{
    "count": 2,
    "next": "https://rodeocode.com/api/projects/?q=admin&page=2",
    "previous": null,
    "results": [
        {
            "id": 1,
            "name": "RodeoCode admin",
            "slug": "rodeocode-admin",
            "active": true,
            "created_at": "2016-03-12T07:53:24Z",
            "team": 1,
            "repositories": [
                1
            ]
        },
        ...
    ]
}
```

Retrieve projects by keyword query. Results are limited to those projects that 
the currently authed user has read permissions to view.

### HTTP Request

`GET https://rodeocode.com/api/projects/search/?q=<urlEncodedQueryString>`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
q | String | [URL-encoded](https://en.wikipedia.org/wiki/Percent-encoding) string to search for projects by name.
