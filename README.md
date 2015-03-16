# Kinja

Ruby gem for posting to Kinja (currently only supports Burner accounts)

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'kinja'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install kinja

## Usage

```ruby
# Create an instance of the kinja client
client = Kinja::Client.new(
  user: "username",
  password: "password"
)

# Create a post
post = client.post(
  headline: '',                       # required
  body: '<p>This is a post</p>',      # required
  status: 'PUBLISHED',                # optional (default is "DRAFT")
  replies: false                      # optional (default is true)
)
```

## Contributing

1. Fork it ( https://github.com/adampash/kinja/fork )
2. Setup .env file with a test burner account
3. Create your feature branch (`git checkout -b my-new-feature`)
4. Commit your changes with tests (`git commit -am 'Add some feature'`)
5. Push to the branch (`git push origin my-new-feature`)
6. Create a new Pull Request
