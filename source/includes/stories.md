# Stories

A story refers to an expected behavior of a software.

The format of a story contains one or more of the following:

- a "Given" statement
- a "When" statement
- a "Then" statement

This syntax is commonly referred to as "[Gherkin](https://cucumber.io/docs/reference#gherkin)",
after the popular behavior-driven development library named 
[Cucumber](https://github.com/cucumber/gherkin).

## Get Stories

```shell
$ curl "https://rodeocode.com/api/stories/"
[
  {
    "id": 1,
    "project_id": 1,
    "given": [
        {
            "id": 1,
            "statement": "I am logged in"
        },
        ...
    ],
    "when": [
        {
            "id": 1,
            "statement": "I click the login button"
        },
        ...
    ],
    "then": [
        {
            "id": 1,
            "statement": "I see a flash message"
        },
        ...
    ],
    "created_at": "Sun, 06 Mar 2016 22:30:08 -0000"
  }
]
```

Retrieve all stories associated with the given project.

### HTTP Request

`GET https://rodeocode.com/api/stories/`


## Get Stories for Project

Retrieve all stories associated with the given project.

### HTTP Request

`GET https://rodeocode.com/api/projects/<project_id>/stories/`
