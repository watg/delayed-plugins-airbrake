# Delayed::Plugins::Airbrake

`delayed_job` exception notification with Airbrake

Originally based on [this gist](https://gist.github.com/granth/2223758) and [this StackOverflow answer](http://stackoverflow.com/questions/12683364/how-to-make-delayed-job-notify-airbrake-when-an-actionmailer-runs-into-an-error).

## Installation

Add this line to your application's Gemfile:

    gem 'delayed-plugins-airbrake'

## Usage

Register the plugin like so:

    require 'delayed/plugins/airbrake'
    Delayed::Worker.plugins << Delayed::Plugins::Airbrake

In a Rails project, this can be done in `config/initializers`.

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
