# Summary

Provides an up-to-date RSS product feed for Google Merchant rather a file that you have to upload. This is a very basic extension so feel free to help improve it!

To test and access the RSS feed visit:
`http://locahost:3000/google_merchant.rss`

## Installation & Usage

To start with you'll need a Google Merchant account. Then, add the gem to your `Gemfile`

```ruby
gem "solidus_google_merchant", github: 'Domenoth/solidus_google_merchant.git', branch: 'solidus-1-1-stable'
```

Then bundle

```ruby
bundle install
```

Next, configure the feed title, description and site URL by browsing to the Google Merchant settings page in `Admin -> Settings`

Finally, set up your products in Solidus by editing the product's properties.  You should add the following properties:

```sh
google_product_type
manufacturer
brand
model
upc
```

## Testing
In order to run the rspec test suite:

```ruby
rake test_app
rake spec
```

Copyright (c) 2014 lordnibbler, released under the New BSD License
