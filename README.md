Ruby client for [Auth0](https://auth0.com)

> This used to be the omniauth strategy for [Auth0](https://auth0.com) but now is a client for the Auth0 api. The omniauth strategy has been moved to [omniauth-auth0](https://github.com/auth0/omniauth-auth0).

## Installation

```
$ gem install auth0
```

## Basic usage

```ruby
require "auth0"

auth0 = Auth0Client.new(
  :client_id => "YOUR CLIENT ID",
  :client_secret => "YOUR CLIENT SECRET",
  :namespace => "<YOUR ACCOUNT>.auth0.com"
);

puts auth0.get_connections;
```

Using [APIv2](https://auth0.com/docs/apiv2)

```ruby
require "auth0"

auth0 = Auth0Client.new(
  :api_version => 2,
  :token => "YOUR JWT HERE"
);

puts auth0.get_users;
```

## License

MIT 2014 - Auth0 INC.
