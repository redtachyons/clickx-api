# locations

## Get All Locations

```ruby
require 'clickx'

api = Kittn::APIClient.authorize!('user-token')
api.locations.get
```

```shell
curl "http://example.com/api/v1/locations"
  -H "X-USER-TOKEN: user-token"
```

> The above command returns JSON structured like this:

```json
{"data":[{"id":"216","type":"locations","attributes":{"name":"Clickx","address":"222 W. Merchandise Mart Plaza, Suite 1212","city":"Chicago","state":"IL","country":"United States","zip":"60654","phone":"312-945-7150","mobile-phone":"","toll-free":"","website":"www.clickx.io","enquiry-email":"","fax":"","categories":[],"payment-methods":[],"products-services":[],"brands":[],"images":[null],"languages":[],"professional-associations":[],"slogan":"","keywords":"","short-description":"","medium-description":"","full-description":"","long-description":"","number-of-users":null,"year-established":null,"user-id":null,"created-at":"2017-01-02T16:04:09.385-06:00","updated-at":"2017-04-08T07:49:23.342-05:00","business-id":27,"local-profile-list":"","local-profile-last-upload":null,"lat":"41.888244","lng":"-87.635388","operational-hours":true,"positive-review-coupon":null,"negative-review-coupon":null,"slug":"clickx","short-url":"https://clickx.ly/2iw59R3","reviews-count":0,"bl-reviews-info":{},"average-rating":null,"contact-name":"Solomon Thimothy"}},{"id":"177","type":"locations","attributes":{"name":"Clickx","address":"8833 Gross Point","city":"Skokie","state":"IL","country":"United States","zip":"60077","phone":"8473271970","mobile-phone":"847-327-1970","toll-free":"","website":"www.clickx.io","enquiry-email":"","fax":"","categories":[],"payment-methods":[],"products-services":[],"brands":[],"images":[null],"languages":[],"professional-associations":[],"slogan":"","keywords":"","short-description":"","medium-description":"","full-description":"","long-description":"","number-of-users":49,"year-established":2006,"user-id":null,"created-at":"2016-09-16T14:22:43.131-05:00","updated-at":"2017-04-24T13:37:24.507-05:00","business-id":27,"local-profile-list":"","local-profile-last-upload":null,"lat":"42.041672","lng":"-87.755095","operational-hours":true,"positive-review-coupon":null,"negative-review-coupon":null,"slug":"clickx-1000","short-url":"https://clickx.ly/2irbXvV","reviews-count":4,"bl-reviews-info":{},"average-rating":3.0,"contact-name":"Layla Ella"}}]}% 
```

This endpoint retrieves all locations.

### HTTP Request

`GET http://example.com/api/v1/locations`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
limit | 50 | Limit number of locations in response

