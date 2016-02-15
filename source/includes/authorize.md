# Authorization

In order to provide integrations with various 3rd party services, 
their are various ways of allowing users to authorize RodeoCode
to access your accounts with those services on your behalf.

## Github

```shell
$ curl "https://rodeocode.com/api/accounts/users/github?scope=projects"
302 Location: https://github.com/...
```

This URL appropriately redirects to the respective Github OAuth endpoint.

### HTTP Request

`GET https://rodeocode.com/api/accounts/users/github?scope=projects`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
scope | None | The desired [scopes](https://developer.github.com/v3/oauth/#scopes) to be authorized

## Bitbucket

```shell
$ curl "https://rodeocode.com/api/accounts/users/bitbucket?scope=projects"
302 Location: https://bitbucket.com/...
```

This URL appropriately redirects to the respective Bitbucket OAuth endpoint.

### HTTP Request

`GET https://rodeocode.com/api/accounts/users/bitbucket?scope=projects`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
scope | None | The desired [scopes](https://confluence.atlassian.com/bitbucket/oauth-on-bitbucket-cloud-238027431.html#OAuthonBitbucketCloud-Scopes) to be authorized

## Gitlab

Coming soon...[or come help us build it](mailto:careers@rodeocode.com)!
