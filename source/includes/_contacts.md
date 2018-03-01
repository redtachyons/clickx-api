# contacts

## Get All Contacts

```ruby
require 'clickx'

api = Kittn::APIClient.authorize!('user-token')
api.contacts.get
```

```shell
curl "http://example.com/api/v1/tracker_contacts"
  -H "X-USER-TOKEN: user-token"
```

> The above command returns JSON structured like this:

```json
[
   {
      "id":"5562",
      "type":"tracker-contacts",
      "attributes":{
         "first-name":"Brad",
         "last-name":"chauhan",
         "email":"test@example.com",
         "organization":null,
         "phone":null,
         "gender":null,
         "status":"contact",
         "avatar":{
            "url":null
         },
         "website":null,
         "source-utm":null
      }
   },
   {
      "id":"5586",
      "type":"tracker-contacts",
      "attributes":{
         "first-name":"John",
         "last-name":"Doe",
         "email":null,
         "organization":null,
         "phone":"3018737452",
         "gender":null,
         "status":"contact",
         "avatar":{
            "url":null
         },
         "website":null,
         "source-utm":null
      }
   },
]
```

This endpoint retrieves all contacts.

### HTTP Request

`GET http://example.com/api/v1/tracker_contacts`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
limit | 50 | Limit number of contacts in response

<aside class="success">
</aside>

## Get a Specific Contact

```ruby
require 'clickx'

api = Kittn::APIClient.authorize!('user-token')
api.contacts.get(2)
```

```shell
curl "http://example.com/api/contacts/2"
  -H "X-USER-TOKEN: user-token"
```

> The above command returns JSON structured like this:

```json
{
"id":5586,
"first_name":"WIRELESS",
"last_name":"CALLER",
"email":null,
"organization":null,
"phone":"3018737452",
"gender":null,
"status":"contact",
"avatar":{"url":null},
"website":null,
"source_utm":null
}  
```

This endpoint retrieves a specific contact.

### HTTP Request

`GET https://app.clickx.io/api/v1/tracker_contacts/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the contact to retrieve


## Create new contact

Create a new contact


### HTTP Request

`POST https://app.clickx.io/api/v1/tracker_contacts`

### Contact Parameters

Parameter | Description
--------- | -----------
name | Full name of the contact
email* | Email of the contact
phone | Phone number of the contact
website | Contact's website

