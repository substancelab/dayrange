# DayRange

`DayRange` provides methods to navigate and manipulate series of dates.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'dayrange'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install dayrange

## Usage

```ruby
year = DayRange.new(Date.new(2022, 1, 1), Date.new(2022, 12, 31))

# Navigate to the period before
last_year = year.previous

# Navigate to the period after
next_year = year.next

# Iterate through the year
year.each do |date|
  # Every day of the year
end

# Iterate in more interesting ways
year.every(weeks: 2) do |date|
  # Every other week of the year
end
```

## Related projects

* https://github.com/moneybird/active-date-range
* https://rubygems.org/gems/cada

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and the created tag, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/substancelab/dayrange.
