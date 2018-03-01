---
title: Clickx API Reference

language_tabs:
  - shell
  - ruby

toc_footers:
  - <a href='https://app.clickx.io'>Clickx</a>

includes:
  - locations
  - agencies
  - notifications
  - competitions
  - errors

search: true
---

# Introduction

Welcome to the Clickx API!.

# Authentication

There are two ways for authentication

* simple Token based authentication
* Oauth2


## Simple Token based authentication


```ruby
require 'net/http'
uri = URI('https://app.clickx.io/api/v1/login')
res = Net::HTTP.post_form(uri, 'email' => '<email>', 'password' => '<password>')
puts res.body
```

```shell
 curl -H "Content-Type: application/json" -X POST -d '{"email":"<email>","password":"<password>"}' https://app.clickx.io/api/v1/login
```


Clickx api expects for the API key to be included in all API requests to the server in a header that looks like the following:

`X-USER-TOKEN: my_token`

<aside class="notice">
You must replace <code>my_token</code> with the token of the corresponding user.
</aside>

## OAuth2

```ruby
require 'oauth2'
site          = "https://app.clickx.io"
client_id     = '<client id>'
client_secret = '<client secret>'
redirect_uri  = '<redirect uri>'

client = OAuth2::Client.new(client_id, client_secret, :site => site)

client.auth_code.authorize_url(:redirect_uri => redirect_uri)

token = client.auth_code.get_token(code, :redirect_uri => redirect_uri)

token.get("/api/v1/users/me")
```
