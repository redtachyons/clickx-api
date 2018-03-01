# Agencies

## Get All Agencies

```ruby
require 'clickx'

```

```shell
curl "http://example.com/api/v1/agencies"
  -H "X-USER-TOKEN: user-token"
```

> The above command returns JSON structured like this:

```json
{"data":[{"id":"2","type":"agencies","attributes":{"name":"Clickx","phone":"888-909-7265","support-email":"support@clickx.io","logo":"https://res.cloudinary.com/hwdkgnvx8/image/upload/v1435069959/agency_logos/admf5qb6oz47q908caok.png","address":"8833 Gross Point,  202, Skokie, IL 60077"}},{"id":"3","type":"agencies","attributes":{"name":"OneIMS","phone":"8473271970","support-email":"support@oneims.com","logo":"https://res.cloudinary.com/hwdkgnvx8/image/upload/v1483997530/agency_logos/u6kgmg47srgi7gocxejq.png","address":"8833 Gross Point, Suite 202, Skokie, IL 60077"}},{"id":"4","type":"agencies","attributes":{"name":"TCompanies, Inc.","phone":"702-425-3100","support-email":"support@clickx.io","logo":null,"address":"405 Max Court #241A Henderson, NV 89011"}},{"id":"5","type":"agencies","attributes":{"name":"Webs We Weave","phone":"847.540.9668","support-email":"support@clickx.io","logo":"","address":"818 Indigo Court, Lake Zurich, IL 60047"}}]}
```

This endpoint retrieves all agencies.

### HTTP Request

`GET http://example.com/api/v1/agencies`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
limit | 50 | Limit number of agencies in response

