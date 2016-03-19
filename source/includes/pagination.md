# Pagination

## Get Paginated Results

Many RodeoCode API endpoints return "lists" of a resource.

In order to efficiently return results, the API returns 25 
results per "page".

To access the next page of results, retrieve the URL for the 
next or previous page as specified by the API endpoints 
response.

If there are no results on the requested page then the API
return a 404 Not Found response.

For an example, please see the [Project list](#get-projects) endpoint.

