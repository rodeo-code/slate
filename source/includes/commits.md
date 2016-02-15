# Commits

## Get Project Commits

```shell
$ curl "https://rodeocode.com/api/projects/1/commits/"
{
  "count": 2,
  "data": [
    {
      "id": 1,
      "commit_hash": "asdfasdf"
    },
    ...
  ]
}
```

Retrieve all commits for the given project.

### HTTP Request

`GET https://rodeocode.com/api/projects/<project_id>/commits/`
