# Treeview

TreeView

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'treeview'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install treeview

## Usage
```
require 'treeview'

dir = [
  {
    :Applications => [
       :'Safari.app'
    ]
  },
  {
    :Users => [
      {
        :mocchi => [
          :bin,:Document
        ]
      }
    ]
  }
] 
puts TreeView::tree(dir)

#|__Applications
#|  \__Safari.app
#\__Users
#   \__mocchi
#         |__bin
#               \__Document
```

## Contributing

1. Fork it ( https://github.com/[my-github-username]/treeview/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
