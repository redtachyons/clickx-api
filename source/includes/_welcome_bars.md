# WelcomeBars

## Get All WelcomeBars

```ruby
require 'clickx'

api = Kittn::APIClient.authorize!('user-token')
api.welcome_bars.get
```

```shell
curl "http://example.com/api/v1/welcome_bars"
  -H "X-USER-TOKEN: user-token"
```

> The above command returns JSON structured like this:

```json
{
  "data":
  [
  {
    "id":"17",
    "type":"hello-bars",
    "attributes":
    {
      "active":true,
      "template":"\u003cdiv id=\"clickx__hellobar\" class=\"clickx_hellobar cx_hello\" style=\"background: rgb(246, 168, 0) none repeat scroll 0% 0%; border-radius: 0px;\"\u003e\u003cdiv id=\"clxh_close\" class=\"clx_h_close\"\u003e\u003cspan id=\"rp-h-close-icon\"\u003e\u003ci style=\"background-color: rgb(196, 111, 111);\"\u003e\u003c/i\u003e\u003ci style=\"background-color: rgb(196, 111, 111);\"\u003e\u003c/i\u003e\u003c/span\u003e\u003c/div\u003e\u003cdiv class=\"clx_h_content\"\u003e\u003cdiv class=\"clx_h_content_img\"\u003e\u003cdiv class=\"clx_h_img_table\"\u003e\u003cdiv class=\"clx_h_img_cell\"\u003e\u003ca class=\"clx_h_img_a\" href=\"http://www.clickx.io?utm_source=http://www.clickx.io\u0026amp;utm_campaign=welcomebar\u0026amp;utm_medium=offerwidget\" target=\"_blank\"\u003e\u003cimg class=\"clx_h_img_tag\" id=\"clx-h-img-tag\" src=\"data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz48c3ZnIHZlcnNpb249IjEuMSIgaWQ9IkxheWVyXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4IiB2aWV3Qm94PSIwIDAgMTQ0IDE3MCIgc3R5bGU9ImVuYWJsZS1iYWNrZ3JvdW5kOm5ldyAwIDAgMTQ0IDE3MDsiIHhtbDpzcGFjZT0icHJlc2VydmUiPjxzdHlsZSB0eXBlPSJ0ZXh0L2NzcyI+LnN0MHtmaWxsOiNGRkZGRkY7fTwvc3R5bGU+PGc+PGc+PHBhdGggY2xhc3M9InN0MCIgZD0iTTg2LjcsNjMuMWM0LDMsOS41LDIuMSwxMi41LTJsMzAuMS00MC44YzMtMy45LDIuMS05LjUtMi0xMi41Yy0zLjktMy05LjUtMi4xLTEyLjUsMkw4NC43LDUwLjZDODEuOSw1NC42LDgyLjcsNjAuMiw4Ni43LDYzLjF6Ii8+PHBhdGggY2xhc3M9InN0MCIgZD0iTTExOS4xLDE2MC43YzMsMy45LDkuMSw0LjQsMTIuNSwxLjhjMy45LTMsNC44LTguNiwxLjgtMTIuNUw5OSwxMDMuM2MtMy0zLjktOC42LTQuOS0xMi41LTJzLTQuOSw4LjYtMiwxMi41TDExOS4xLDE2MC43eiIvPjxwYXRoIGNsYXNzPSJzdDAiIGQ9Ik03OC4zLDc2LjhMNTUuMSw0NS40TDI4LjksOS45Yy0zLTMuOS04LjYtNC45LTEyLjUtMmMtMy45LDMtNC45LDguNi0yLDEyLjVsNDEuMSw1NS44bDAuNSwwLjdjMi41LDMuMywyLjMsNy45LDAsMTEuMmwtNDUuOCw2MmMtMywzLjktMi4xLDkuNSwyLDEyLjVjMy45LDMsOS41LDIuMSwxMi41LTJsNTMuOC03My4xQzgwLjMsODUuMiw4MS4yLDgwLjYsNzguMyw3Ni44eiIvPjwvZz48L2c+PC9zdmc+\"\u003e\u003c/a\u003e\u003c/div\u003e\u003c/div\u003e\u003c/div\u003e\u003cdiv class=\"clx_h_title\" style=\"text-align: center;\"\u003eGet on the Map: 3 Strategies to \nFuture Proof Your Local Marketing [Live Training]\u003cform class=\"clx-h-form\" action=\"http://localhost:3000/welcome_bar_form_data\" method=\"POST\"\u003e\u003cinput placeholder=\"Enter your Email address\" class=\"clx-h-input\" name=\"welcome_bar[email]\" required=\"required\" type=\"text\"\u003e\u003cinput class=\"clx-h-input\" name=\"welcome_bar[welcome_bar_id]\" type=\"hidden\"\u003e\u003cbutton class=\"clx-h-submit\" type=\"submit\"\u003eSubmit\u003c/button\u003e\u003c/form\u003e\u003ca class=\"clx_h_link\" id=\"clx_h_link_id\" target=\"_blank\" href=\"https://offers.clickx.us/webinar-registration-3-strategies-to-future-proof-your-local-marketing-webinar\" style=\"background: rgb(255, 255, 255) none repeat scroll 0% 0%; margin-left: 15px; padding: 3px 19px; border-radius: 17px;\"\u003eRegister\u003c/a\u003e\u003c/div\u003e\u003c/div\u003e\u003c/div\u003e"}}]}
```

This endpoint retrieves all welcome_bars.

### HTTP Request

`GET http://example.com/api/v1/welcome_bars`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
limit | 50 | Limit number of welcome_bars in response

