### What's this?

Forked from [sample slack-ruby-bot-server](https://github.com/slack-ruby/slack-ruby-bot-server/tree/master/sample_apps/sample_app_activerecord)
This is a sample slack-ruby-bot-server with ActiveRecord.

### Setup

To run samples, [register a new Slack app](https://api.slack.com/apps), configure a bot user, and OAuth redirect URL to http://localhost:9292 (for development).

Set the below envars:

```
SLACK_CLIENT_ID=1111111111.2222222
SLACK_CLIENT_SECRET=abcdef012345679
PORT=9292
```

Run tests with `bundle exec rake`.



### Run

```
bundle install
rake db:create db:migrate
RAILS_ENV=test rake db:migrate
rackup
```
