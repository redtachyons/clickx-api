# Notifications

## Get All Notifications

```ruby
require 'clickx'

api = Kittn::APIClient.authorize!('user-token')
api.notifications.get
```

```shell
curl "http://example.com/api/v1/notifications"
  -H "X-USER-TOKEN: user-token"
```

> The above command returns JSON structured like this:

```json
{
  "data":[
  {
    "id":"9",
    "type":"notifications",
    "attributes":
    {
      "content":"New contact khh  created in Clickx",
      "read-at":null,
      "view-path":"/notifications/9/view",
      "created-at":"2017-04-26T23:56:16.031-05:00"
    }
  },
  {
    "id":"21",
    "type":"notifications",
    "attributes":
    {
      "content":"New contact   created in Clickx",
      "read-at":null,
      "view-path":"/notifications/21/view",
      "created-at":"2017-04-27T00:53:36.663-05:00"
    }
   },
   {
      "id":"33",
      "type":"notifications",
      "attributes":
      {
        "content":"New contact   created in Clickx",
        "read-at":null,
        "view-path":"/notifications/33/view",
        "created-at":"2017-04-27T00:55:03.642-05:00"}
      },
      {
        "id":"45","type":"notifications",
        "attributes":{
          "content":"New contact   created in Clickx",
          "read-at":null,
          "view-path":"/notifications/45/view",
          "created-at":"2017-04-27T00:55:52.773-05:00"
      }
    }
  ]
}
```

This endpoint retrieves all notifications.

### HTTP Request

`GET http://example.com/api/v1/notifications`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
limit | 50 | Limit number of notifications in response

