# Steps

## Get Steps

```shell
$ curl "https://rodeocode.com/api/project/1/features/1/steps/"
{
    "count": 2,
    "next": null,
    "previous": null,
    "results": [
        {
            "id": 1,
            "priority": 0,
            "step_type": 0,
            "regex": "I am logged in",
            "active": true,
            "created_at": "2016-03-14T08:55:53.927736Z",
            "scenario": 1
        }
        ...
    ]
}
```

Retrieve all steps for a given scenario.

### HTTP Request

`GET https://rodeocode.com/api/projects/<project_id>/features/<feature_id>/scenarios/<scenario_id>/steps/`


## Create a Step

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/scenarios/1/steps/"
  -X POST
  -d @- <<REQUEST_BODY
{
    "priority": 0,
    "step_type": 0,
    "regex": "I am logged in",
    "scenario": 1
}
REQUEST_BODY
```

Create a new step.

### HTTP Request

`POST https://rodeocode.com/api/projects/<project_id>/features/<feature_id>/scenarios/<scenario_id>/steps/`


## Get a Step

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/scenarios/1/steps/1/"
  -X GET
{
    "id": 1,
    "priority": 0,
    "step_type": 0,
    "regex": "I am logged in",
    "active": true,
    "created_at": "2016-03-14T08:55:53.927736Z",
    "scenario": 1
}
```

Get an existing step.

### HTTP Request

`GET https://rodeocode.com/api/projects/<projectId>/features/<feature_id>/scenarios/<scenario_id>/steps/<step_id>/`


## Update a Step

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/scenarios/1/steps/1/"
  -X PATCH
  -d @- <<REQUEST_BODY
{
    "step_type": 1,
    "regex": "I am not logged in"
}
REQUEST_BODY
```

Update an existing step.

### HTTP Request

`PATCH https://rodeocode.com/api/projects/<projectId>/features/<feature_id>/scenarios/<scenario_id>/steps/<step_id>/`


## Deleting a Scenario

```shell
$ curl "https://rodeocode.com/api/projects/1/features/1/scenarios/1/steps/1/"
  -X PATCH
  -d @- <<REQUEST_BODY
{
    "active": false
}
REQUEST_BODY
```

Delete an existing step.

### HTTP Request

`PATCH https://rodeocode.com/api/projects/<projectId>/features/<feature_id>/scenarios/<scenario_id>/steps/<step_id>/`
