# Scenarios

## Get Scenarios

```shell
$ curl "https://rodeocode.com/api/project/1/features/"
{
    "count": 2,
    "next": null,
    "previous": null,
    "results": [
        {
            "id": 1,
            "name": "Click the logout button",
            "active": true,
            "created_at": "2016-03-14T08:44:02.040688Z",
            "feature": 1
        }
        ...
    ]
}
```

Retrieve all scenarios for a given project feature.

### HTTP Request

`GET https://rodeocode.com/api/projects/<project_id>/features/<feature_id>/scenarios/`


## Create a Feature

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/scenarios/"
  -X POST
  -d @- <<REQUEST_BODY
{
    "name": "Click the logout button"
}
REQUEST_BODY
```

Create a new feature.

### HTTP Request

`POST https://rodeocode.com/api/projects/<project_id>/features/<feature_id>/scenarios/`


## Get a Feature Scenario

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/scenarios/1/"
  -X GET
{
    "id": 1,
    "name": "Test",
    "active": true,
    "created_at": "2016-03-14T08:44:02.040688Z",
    "feature": 1
}
```

Get an existing scenario.

### HTTP Request

`GET https://rodeocode.com/api/projects/<projectId>/features/<feature_id>/scenarios/<scenario_id>/`


## Update a Scenario

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/scenarios/1/"
  -X PATCH
  -d @- <<REQUEST_BODY
{
    "name": "Modified name"
}
REQUEST_BODY
```

Update an existing scenario.

### HTTP Request

`PATCH https://rodeocode.com/api/projects/<projectId>/features/<feature_id>/scenarios/<scenario_id>/`


## Deleting a Scenario

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/scenarios/1/"
  -X PATCH
  -d @- <<REQUEST_BODY
{
    "active": false
}
REQUEST_BODY
```

Delete an existing scenario.

### HTTP Request

`PATCH https://rodeocode.com/api/projects/<projectId>/features/<feature_id>/scenarios/<scenario_id>/`
